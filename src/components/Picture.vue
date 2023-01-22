<template>
  <img :src="avatar" :alt="descricao"/>
  <Reutilizacao/>
</template>

<script>
  import Reutilizacao from "@/components/Reutilizacao";
  export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Picture',
    components: {Reutilizacao},
    data() {
      return{
        avatar: "/img/deb.png",
        descricao: "Vasco Teixeira"
      }
    }
  }
</script>