<template>
  <PrimeiroComponente/>
  O dado de app é {{ testando }}
  <LifeCycle/>
  <Pessoa/>
</template>

<script>

import PrimeiroComponente from "@/components/PrimeiroComponente";
import LifeCycle from "@/components/LifeCycle";
import Pessoa from "@/components/Pessoa";

export default {
  name: 'App',
  components: {
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