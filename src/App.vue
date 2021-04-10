<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!-- <maincomponent  /> -->
    <fetchApi />
  </div>
</template>

<script>
// import maincomponent from './components/maincomponent.vue'
import fetchApi from './components/fetchApi'

export default {
  name: 'App',
  components: {
    // maincomponent
    fetchApi
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
