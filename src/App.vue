<template>
  <PageHeader
      v-if="showHeader"
  />

  <div
      v-for="obj in todos"
      v-bind:key="obj.id"
      class="tomilho"
  >
    {{ obj.title }}
  </div>

  <img
      alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import PageHeader from './components/PageHeader.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    PageHeader
  },
  // Central de variaveis do componente
  data(){
    return{
      showHeader: true,

      todos: [
        {
          "userId": 1,
          "id": 1,
          "title": "delectus aut autem",
          "completed": false
        },
        {
          "userId": 1,
          "id": 2,
          "title": "quis ut nam facilis et officia qui",
          "completed": false
        },
        {
          "userId": 1,
          "id": 3,
          "title": "fugiat veniam minus",
          "completed": false
        },
        {
          "userId": 1,
          "id": 4,
          "title": "et porro tempora",
          "completed": true
        },
        {
          "userId": 1,
          "id": 5,
          "title": "laboriosam mollitia et enim quasi adipisci quia provident illum",
          "completed": false
        }
      ]

      }
    }
  }
</script>

<style>
.tomilho{
  background-color: #000;
  margin: 5px 50px 5px 50px;
  padding: 3px 6px;
  color: #fff;
  text-align: left;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 60px;
}
</style>
