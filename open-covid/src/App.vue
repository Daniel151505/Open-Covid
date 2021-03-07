<template>
  <div id="app">
<Bienvenida/>
  </div>
</template>

<script>
import Bienvenida from './components/Bienvenida.vue'

export default {
  name: 'App',
  components: {
    Bienvenida
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
