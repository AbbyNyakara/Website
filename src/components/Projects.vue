<template>
  <div class="projects">
    <div class="projects__top">
      <div>
        <h2 class="projects__title"> Projects</h2>
      </div>
      <div>
        <a href="">Contact Me</a>
      </div>
    </div>
    
  </div>
</template>

<script>
  export default {
    name: "Projects"
  }
</script>

<style scoped>
  .projects {
    position: absolute;
    top: 200vh;
    margin-top: 2rem;
    width: 80%;
  }

  .projects__title {
    font-size: 6rem;
  }

   a {
    color: inherit;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    border-bottom: 3px solid rgb(78, 225, 160);
  }

  .projects__top {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>