<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <router-link to="/A">Go to componentA</router-link>
    <router-link to="/B">Go to componentB</router-link>
    <router-link to="/C">Go to componentC</router-link>
    <router-view></router-view>
  </div>
</template>

<script>

export default {
  name: 'hello',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
    }
  },
  components: {
  },
  methods: {
    
  },
  created() {
    
  },
}
</script>

