<template>
  <div id="app">
    
    <Navbar/>
    <Slider/>
    <Idea/>
    <Team/>
    <Footer/>
<Bienvenida/>
  </div>
</template>

<script>
import Bienvenida from './components/Bienvenida.vue'
import Topbar from './components/Topbar.vue'
import Navbar from './components/Navbar.vue'
import Slider from './components/Slider.vue'
import Idea from './components/Idea.vue'
import Team from './components/Team.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Bienvenida,
    Topbar,
    Navbar,
    Slider,
    Idea,
    Team,
    Footer
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
