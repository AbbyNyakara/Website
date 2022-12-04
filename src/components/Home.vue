<template>
  <div class="home">
    <img src="../assets/images/pattern-rings.svg" class="top__rings" alt="">
    <div class="home__body">
      <h1>Nice to meet you! <br> I'm <span>Abby Nyakara.</span></h1>
      <div class="intro_text">
        Based in Kenya, I'm a full-stack developer <br> passionate about building accesible applications <br> that meet the users' needs.
      </div> 
    </div>
    <a href="">Contact Me</a>
  </div>
</template>

<script>
  export default {
    name: "Home"
  }
</script>

<style scoped>
  .home {
    position: relative;
  }

  h1 {
    font-size: 5rem;
  }

  span {
    border-bottom: 8px solid rgb(78, 225, 160);
    padding-bottom: 5px;
  }

  .intro_text {
    padding-top: 4rem;
    font-size: 1.1rem;
  }

  .top__rings {
    position: absolute;
    top: 25px;
    left: -20%;
  }

  .home__body {
    position: absolute;
    top: 80px;
  }

  a {
    position: absolute;
    top: 450px;
    color: inherit;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    border-bottom: 3px solid rgb(78, 225, 160);
    padding-bottom: 8px;
  }

  
</style>