<template>
  <form action="" @submit="enviarFormulario($event)">
    <input type="text" v-model="name"/>
    <input type="text" v-model="email"/>
    <submit/>
  </form>
  <p>Conteudo</p>
  <p>Conteudo</p>
  <p>Conteudo</p>
</template>
<script>
  import Submit from "@/components/Form/Submit";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Form',
  components: {
    Submit
  },
  data(){
    return{
      name: '',
      email: ''
    }
  },
  methods: {
    enviarFormulario(e){
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("Form enviado");
      console.log("O nome é: " + name);
      console.log("O email é: " + email);

    }
  }
}
</script>

<style scoped>
p{
  margin: 150px;
}
</style>