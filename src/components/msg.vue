<template>
    <div class="msg">
        <span style="color:red;">{{ love }}</span>
  </div>
</template>

<script>
export default {
  name: 'msg',
  props: ['love'],
  data () {
    return {
      
    }
  },
  methods: {
      
  },
  watch: {
    love(newVal,oldVal){
      console.log("megValChange");
    }
  }
}
</script>

<style>

</style>
