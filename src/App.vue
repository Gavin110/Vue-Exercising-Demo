<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <!-- <h1>{{ msg }}</h1>
    <router-link to="/A">Go to componentA</router-link>
    <router-link to="/B">Go to componentB</router-link>
    <router-link to="/C">Go to componentC</router-link> -->
    <cart-nav></cart-nav>
    <!-- 路由外链 -->
    <router-view></router-view>
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import store from './vuex/store'
export default {
  name: 'app',
  store,
  data() {
    return {
      msg: 'Welcome to Your Vue App!',
    }
  },
  components: {
    'cart-nav': Nav
  },
  methods: {
    
  },
  created() {
    
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
