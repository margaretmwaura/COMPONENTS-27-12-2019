<template>
  <div id="app">
    <navigation v-bind:navigations="navigations"/>
    <banner></banner>
    <learnmore @finished="finished">
      <p>{{slotmsg}}</p>
    </learnmore>
    <tablayout></tablayout>
  </div>
</template>
<script>
  import learnmore from './components/learnmore'
  import navigation from './components/navigation'
  import banner from "./components/banner";
  import tablayout from "./components/tabslayout";
export default {
  name: 'app',
  components: {
    banner,
    navigation,
    learnmore,
    tablayout,
  },
  data (){
    return {
      navigations: [
        {name: 'The Company'},
        {name: 'Our Team'},
        {name: 'Our Solutions'},
        {name: 'Media'},
        {name: 'Contact'},
      ],
      slotmsg : " "
    }
  },
  methods : {
    finished() {
      this.slotmsg = 'The documentation is loading .. please wait'
    }}
}
</script>
<style lang="scss">
  @import "../foundation/css/app.css";
  @import "../foundation/css/foundation.css";
  @import "./styles/_variables.scss";
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
  }
</style>
