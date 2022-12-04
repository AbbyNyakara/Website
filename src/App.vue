<template>
  <div class="app">
    <Navbar />
    <Home />
    <Skills />
    <Projects />
  </div>
</template>

<script>
  import Navbar from './components/Navbar.vue';
  import Home from './components/Home.vue';
  import Skills from './components/Skills.vue';
  import Projects from './components/Projects.vue';

  export default {
    name: 'App',
    components: {
      Navbar,
      Home,
      Skills,
      Projects
    }
  }

</script>

<style scoped>
  .app {
    width: 80%;
    margin: auto;
    color: #fff;
  }
</style>
