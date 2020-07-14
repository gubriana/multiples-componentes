<template>
  <div id="app">
    <a href="https://www.freepik.es/fotos-vectores-gratis/viajes" target="_blank"><img alt="Vue logo" src="./assets/logo.png"></a>
    <GListas titulo="Paises a los que quiero viajar" v-bind:enlaces="Paises_Si"/>
    <GListas titulo="Paises a los que no quiero viajar" v-bind:enlaces="Paises_No"/>
  </div>
</template>
<script>
  import GListas from './components/GListas.vue'
  export default {
    name: 'App',
    components: {
      GListas
    },
    data: () => {
      return {
        Paises_Si:[
          {texto:"Japón",url:"http://japon.jp/"},
          {texto:"Islandia",url:"http://www.islandia.is"},
          {texto:"Noruega",url:"https://en.wikipedia.org/wiki/Norway"},
          {texto:"Suecia",url:"http://www.sweden.se"},
          {texto:"Turquia",url:"https://en.wikipedia.org/wiki/Turquia"},
          {texto:"India",url:"https://en.wikipedia.org/wiki/India"}
        ],
        Paises_No:[
          {texto:"Estados Unidos",url:"https://en.wikipedia.org/wiki/Usa"},
          {texto:"Perú",url:"https://en.wikipedia.org/wiki/Peru"},
          {texto:"China",url:"https://en.wikipedia.org/wiki/China"},
          {texto:"Francia",url:"http://www.france.fr"}
        ]
      };
    }
  };
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
© 2020 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About
