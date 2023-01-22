<template>
  <div>
    <Picture/>
    <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias para backend:</p>
    <ul>
      <li v-for="(technology, index) in backend_tech" v-bind:key="index">{{ technology }}</li>
    </ul>
    <p>Utilizo as seguintes tecnologias para frontend:</p>
    <ul>
      <li v-for="technology in frontend_tech" :key="technology.id">
        {{ technology.language }}
      </li>
    </ul>
    <div>
      <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p class="teste">Para acessar meu portfólio <a target="_blank" v-bind:href="meu_link">Clique aqui</a></p>
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
    return {
      esta_trabalhando: true,
      mostrar_email: false,
      textoBotao: 'Mostrar e-mail',
      email: 'vasco.teixeira@gmail.com',
      meu_link: 'https://google.com',
      backend_tech: ['JavaScript', 'PHP', 'Python'],
      frontend_tech: [
        {id: 1, language: 'HTML'},
        {id: 2, language: 'CSS'},
        {id: 3, language: 'VUE'}
      ]
    }
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email
      if (!this.mostrar_email) {
        this.textoBotao = 'Mostrar e-mail'
      } else {
        this.textoBotao = 'Esconder e-mail'
      }
    }
  }
}
</script>

<style>
.paragrafo-pai {
  color: red;
}
</style>