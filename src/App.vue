<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Estas son dos listas:"/>
    <ListaTech/>
    <ListaFinancial/>
  </div>
</template>

<script>

import ListaTech from './components/ListaTech.vue'
import ListaFinancial from './components/ListaFinancial.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ListaTech,
    ListaFinancial
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