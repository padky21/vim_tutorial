<template>
  <PrimeiroComponente/>
  O dado de app é {{testando}}
</template>

<script>
  import PrimeiroComponente from "@/components/PrimeiroComponente";
  export default{
    name: 'App',
    components: {
      PrimeiroComponente

    },
    data() {
      return{
        testando: "teste"
      }
    }
  }
</script>