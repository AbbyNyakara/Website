<template>
  <div class="app">
    <Navbar />
    <Home />
    <Projects />
    <Skills />
    <Contact />
    <Navbar />
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
      // Home,
      Projects,
      // Skills,
      // Contact,
    }
  }

</script>

<style>
  .app {
    color: #fff;
    width: 100%;
    background-color: hsl(0, 0%, 8%);
    padding: 50px;
    /* Added the following */
    position: absolute;
    overflow: visible;
    padding-top: 0;
  }
</style>
