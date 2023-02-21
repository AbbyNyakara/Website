<template>
  <div class="home">
    <div class="home__body">
      <h1>Nice to meet you! <br> I'm <span>Abby Nyakara.</span></h1>
      <div class="intro_text">
        Based in Kenya, I'm a full-stack developer <br> passionate about building accesible applications <br> that meet the users' needs.
      </div> 
    </div>
    <div class="home__contact">
      <a href="">Contact Me</a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Home"
  }
</script>

<style scoped>
  .home {
    min-height: 75vh;
    text-align: center;
  }

  h1 {
    font-size: 4rem;
    background-color: transparent;
  }

  span {
    border-bottom: 8px solid rgb(78, 225, 160);
    padding-bottom: 5px;
  }

  .intro_text {
    padding-top: 4rem;
    font-size: 1.1rem;
  }

  .home__body {
    padding-top: 4rem;
  }

  .home__contact {
    margin-top: 2rem;
    margin-bottom: 3rem;
  }

  a {
    margin-top: 2rem;
    color: inherit;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    border-bottom: 3px solid rgb(78, 225, 160);
    padding-bottom: 8px;
  }

  @media only screen and (max-width: 960px) {
    .home {
      text-align: center;
      padding-bottom: 2rem;
    }

    h1 {
      font-size: 2rem;
    }
  }
</style>
