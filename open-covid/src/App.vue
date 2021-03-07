<template>
  <div id="app">
<Registro/>
  </div>
</template>

<script>
import Registro from './components/Registro.vue'

export default {
  name: 'App',
  components: {
    Registro
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
