<template>
  <div>
    <Reutilizacao/>
    <h1>Ola vue!</h1>
    <Reutilizacao/>
    <p>Meu nome é {{nome}} e trabalho como {{profissao}}</p>
    <MultiplosEventos/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
    <Reutilizacao/>
  </div>
</template>

<script>
  import MultiplosEventos from './MultiplosEventos.vue'
  import Reutilizacao from "@/components/Reutilizacao";
  export default {
    name: 'PrimeiroComponente',
    components: {
      Reutilizacao,
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