<template>
  <h1 class="title">Vue 3</h1>

  <div>
    <label>Nome</label>
    <br>
  </div>
  <input
      v-model="name"
      type="text"
  >
  <br>
  {{ name }}
  <br>
  <br>
  <div>
    <label>Sports</label><br>
    <select v-model="sports">
      <option value="">Escolha</option>
      <option value="futebol">Futebol</option>
      <option value="skate">Skate</option>
      <option value="basquete">Basquete</option>
    </select><br>
    {{sports}}
  </div>
<br><br>
  <div>
    <label>Newsletter</label>
    <input
        v-model="newsletter"
        type="radio"
        value="Sim"
    >Sim

    <input
        v-model="newsletter"
        type="radio"
        value="Não"
    >Não<br>
    {{newsletter}}
  </div>
  <br><br>
  <div>
    <input
        v-model="colors"
        type="checkbox"
        value="Amarelo"
    > Amarelo
    <input
        v-model="colors"
        type="checkbox"
        value="Azul"
    > Azul
    <input
        v-model="colors"
        type="checkbox"
        value="Verde"
    > Verde
    <input
        v-model="colors"
        type="checkbox"
        value="Roxo"
    > Roxo
  </div>
  <br>
  {{colors}}

</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import PageHeader from './components/PageHeader.vue'

export default {
  name: 'App',

  components: {
    // Importar componentes
  },
  // Central de variaveis do componente
  data() {
    return {
      name: 'Cleber falcão',
      sports: '',
      newsletter: '',
      colors: [],
      users: [
        {
          "id": 1,
          "nome": "Heitor Santos",
          "imgSrc": 'https://placehold.co/150x150'
        },
        {
          "id": 2,
          "nome": "Douglas Santos",
          "imgSrc": 'https://placehold.co/150x150'
        },
        {
          "id": 3,
          "nome": "Vanessa Santos",

        }
      ]

    }
  }
}
</script>

<style>
.title {
  font-size: 20px;
  color: #42b983;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
