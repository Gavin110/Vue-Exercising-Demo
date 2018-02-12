<template>
    <div class="footer">
        footer
    </div>
</template>

<script>
// import bus from './bus.js'

export default {
  name: 'footer',
  data () {
    return {
      msg: 'hi'
    }
  },
  created () {
      this.$root.bus.$on('change',(data)=>{
      console.log(data);
    })
  }
}
</script>

<style>

</style>