<template>
  <nav class="navbar">
    <div class="navbar_logo">
      <p>abbyNyakara</p>
    </div>
    <ul class="navbar_links">
      <li><a href="https://github.com/AbbyNyakara" target="_blank">
        <img src="../assets/images/icon-github.svg" alt="">
      </a></li>
      <li><a href="https://www.frontendmentor.io/profile/AbbyNyakara" target="_blank">
        <img src="../assets/images/icon-frontend-mentor.svg" alt="">
      </a></li>
      <li><a href="https://www.linkedin.com/in/abigael-nyakara/" target="_blank">
        <img src="../assets/images/icon-linkedin.svg" alt="">
      </a></li>
    </ul>
  </nav>
</template>

<script>
  export default {
    name: "Navbar"
  }
</script>

<style scoped>
  nav {
    padding-top: 2rem;
    padding-bottom: 1.5rem;
    display: flex;
    justify-content: space-between;
    position: sticky;
    top: 0;
    width: 100%;
    background-color: hsl(0, 0%, 8%);
    z-index: 1000;
  }

  .navbar_logo p {
    font-size: 1.7rem;
    font-weight: 600;
  }

  .navbar_links {
    display: flex;
    gap: 1rem;
  }

  .navbar_links img:hover {
    fill: rgb(78, 225, 160);
  }

  @media screen and (max-width: 600px) {
    nav {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 2rem;
      font-size: 1.2rem;
    }
  }

</style>