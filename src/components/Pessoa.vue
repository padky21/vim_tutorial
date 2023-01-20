<template>
  <h2>Esta descrição é da pessoa: {{nome}}</h2>
  <Info/>
  <Form/>
</template>
<script>
  import Info from "@/components/Info";
  import Form from "@/components/Form";
  export default{
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Pessoa',
    components: {
      Form,
      Info
    },
    data(){
      return{
        nome: 'Vasco'
      }
    }
  }
</script>