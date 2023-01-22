<template>
  <div>
    <Picture/>
    <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias:</p>
    <ul>
      <li>JS</li>
      <li>C++</li>
      <li>Python</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para: {{email}}</p>
    <p>Para acessar meu portfólio <a target="_blank" v-bind:href="meu_link">Clique aqui</a></p>
  </div>
</template>
<script>
import Picture from "@/components/Picture";
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Info',
  components: {
    Picture
  },
  data() {
    return{
      esta_trabalhando: true,
      mostrar_email: true,
      email: 'vasco.teixeira@gmail.com',
      meu_link:'https://google.com'
    }
  }
}
</script>