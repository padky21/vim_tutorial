<template>
  <div>
    <h1>Ola vue!</h1>
    <p>Meu nome é {{nome}} e trabalho como {{profissao}}</p>
    <MultiplosEventos/>
  </div>
</template>

<script>
  import MultiplosEventos from './MultiplosEventos.vue'
  export default {
    name: 'PrimeiroComponente',
    components: {
      // eslint-disable-next-line vue/no-unused-components
      MultiplosEventos
    },
    data(){
      return{
        nome: "Vasco",
        profissao: "Programador"
      }
    }
  }
</script>