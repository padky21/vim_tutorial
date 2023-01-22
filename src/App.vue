<template>
  <Header :esta_logado="true"/>
  <PrimeiroComponente/>
  <p class="paragrafo-pai">O dado de app é {{ testando }}</p>
  <LifeCycle/>
  <Pessoa/>
  <h1>Terminado!</h1>
</template>

<script>

import PrimeiroComponente from "@/components/PrimeiroComponente";
import LifeCycle from "@/components/LifeCycle";
import Pessoa from "@/components/Pessoa";
import Header from "@/components/Header";

export default {
  name: 'App',
  components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
    // eslint-disable-next-line vue/no-unused-components
    Pessoa

  },
  data() {
    return {
      testando: "teste"
    }
  }
}
</script>

<style>
body{
  background-color: #333;
  color: #fff;
}

a{
  color: red;
}

.teste{
  background-color: black;
}
</style>