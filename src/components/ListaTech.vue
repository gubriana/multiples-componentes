<template>
        <div id = "app">
            <h1 v-if = "tech">Lista de {{ nombre }} de tecnologías que quiere aprender:</h1>
            <ul>
                <li v-for = "(techs, i) in tech" v-bind:key="i" >{{techs}}</li>
            </ul>
        </div>
</template>

<script>
export default {
  name: 'ListaTech',
  data:function() {
    return{
      nombre: "Gabriela",
      tech: true,
      tech: ['HTML', 'CSS', 'Vue', 'Firebase',] 
    }
  }  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
