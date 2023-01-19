<template>
  <div>
    <h1>Ola vue!</h1>
    <p>Meu nome é {{nome}} e trabalho como {{profissao}}</p>
  </div>
</template>

<script>
  export default {
    name: 'PrimeiroComponente',
    data(){
      return{
        nome: "Vasco",
        profissao: "Programador"
      }
    }
  }
</script>