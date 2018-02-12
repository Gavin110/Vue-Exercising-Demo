<template>
    <div class="page">
        page
        <button @click="changeMsg">click</button>
        <div class="contentShopping">
          <keep-alive>
            <router-view v-if="$route.meta.keepAlive"></router-view>
          </keep-alive>
          <router-view v-if="!$route.meta.keepAlive">
          </router-view>
        </div>
    </div>
    
</template>

<script>
import msg from './msg.vue'
// import bus from './bus.js'
import footer from './footer.vue'

export default {
  name: 'page',
  components: { msg,footer },
  data () {
    return {
      message: 'hi'
    }
  },
  methods: {
    changeMsg () {
      this.$root.bus.$emit('change', '666');
    }
  }
}
</script>

<style>

</style>