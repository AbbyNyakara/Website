<template>
  <div class="app">
    <Navbar />
    <Home />
    <Skills />
    <Projects />
    <Contact />
    <Navbar class="bottom__nav" />
  </div>
</template>

<script>
  import Navbar from './components/Navbar.vue';
  import Home from './components/Home.vue';
  import Skills from './components/Skills.vue';
  import Projects from './components/Projects.vue';
  import Contact from './components/Contact.vue';

  export default {
    name: 'App',
    components: {
      Navbar,
      Home,
      Skills,
      Projects,
      Contact
    }
  }

</script>

<style scoped>
  .app {
    width: 80%;
    margin: auto;
    color: #fff;
  }

  .bottom__nav {
    position: absolute;
    top: 440vh;
    display: flex;
    justify-content: space-between;
  }
</style>
