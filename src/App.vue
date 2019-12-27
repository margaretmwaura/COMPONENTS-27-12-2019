<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <pratice></pratice>
  </div>
</template>

<script>
  import pratice from './components/pratice'

export default {
  name: 'app',
  components: {
    pratice
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
