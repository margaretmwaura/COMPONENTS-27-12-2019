<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <pratice></pratice>
    <listusingprops v-bind:artists = "artists"/>
  </div>
</template>

<script>
  import pratice from './components/pratice'
  import listusingprops from './components/listusingprops'
export default {
  name: 'app',
  components: {
    pratice,
    listusingprops
  },
  data (){
    return {
      artists: [
        {name: 'Davido', genre: 'afrobeats', country: 'Nigeria'},
        {name: 'Burna Boy', genre: 'afrobeats', country: 'Nigeria'},
        {name: 'AKA', genre: 'hiphop', country: 'South-Africa'},
        {name: 'Sarkodie', genre: 'hiphop', country: 'Ghana'},
        {name: 'Stormzy', genre: 'hiphop', country: 'United Kingdom'},
        {name: 'Lil Nas', genre: 'Country', country: 'United States'},
        {name: 'Nasty C', genre: 'hiphop', country: 'South-Africa'},
        {name: 'Shatta-walle', genre: 'Reagae', country: 'Ghana'},
        {name: 'Khalid', genre: 'pop', country: 'United States'},
        {name: 'ed-Sheran', genre: 'pop', country: 'United Kingdom'}
      ]
    }
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
