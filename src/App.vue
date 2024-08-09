<template>
  <h1 class="title">Vue 3</h1>

  <p>
    
  </p>

  <div
      v-for="(obj, index) in users"
      v-bind:key="obj.id"
      class="tomilho"
  >
    <img
        v-if="obj.imgSrc"
        v-bind:src="obj.imgSrc"
    >
    {{index}} - {{ obj.nome }}
  </div>

</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import PageHeader from './components/PageHeader.vue'

export default {
  name: 'App',
  components: {

  },
  // Central de variaveis do componente
  data(){
    return{

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
.title{
  font-size: 20px;
  color: #42b983;
}
.tomilho{
  display: flex;
  background-color: #000;
  margin: 5px 50px 5px 50px;
  padding: 3px 6px;
  color: #fff;
  align-items: center;
}

.tomilho_img{

}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
