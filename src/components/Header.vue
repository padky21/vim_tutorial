<template>
<ul>
  <li><a href="#">Home</a></li>
  <li><a href="#">Projetos</a></li>
  <li><a href="#">Contato</a></li>
  <li v-if="esta_logado"><a href="#">Meu perfil</a></li>
</ul>
</template>
<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Header',
  props: ["esta_logado"]
}
</script>

<style scoped>
ul{
  list-style: none;
  display: flex;
}
li{
  margin-right: 10px;
}

a{
  color: #ddd;
  text-decoration: none;
  transition: .5s;
}
a:hover{
  color: turquoise;
}
</style>