<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld />
  <MyHome/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyHome from './components/MyHome.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    MyHome
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
