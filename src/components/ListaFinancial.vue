<template>
        <div id = "app">
            <h1 v-if = "financial">Lista de {{ nombre }} de tematicas financieras que quiere aprender:</h1>
            <ul>
                <li v-for = "(financials, i) in financial" v-bind:key="i" >{{financials}}</li>
            </ul>
        </div>
</template>

<script>
export default {
  name: 'ListaFinancial',
  data:function() {
    return{
      nombre: "Gabriela",
      financial: true,
      financial: ['investing', 'budgeting', 'balancing or checkbook'] 
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
