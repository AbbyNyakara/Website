<template>
  <div class="projects">
    <div class="projects__top">
      <div>
        <h2 class="projects__title"> Projects</h2>
      </div>
      <div>
        <a href="#">Contact Me</a>
      </div>
    </div>
    <div class="projects__cards">
      <div class="project__card">
        <div>
          <div class="project__img">
            <img src="../assets/images/thumbnail1.webp" alt="">
            <span class="image__overlay">
              <div class="project__links">
                <a href="" target="_blank">View Project</a>
                <a href="" target="_blank">View Code</a>
              </div>
            </span>
          </div>
          
        </div>
        
        <div class="project__details">
          <h3>TODO WEB APP</h3>
          <ul class="project__lang">
            <li>Vue-JS</li>
            <li>Vitest</li>
            <li>CSS</li>
          </ul>
        </div>
      </div>
      <div class="project__card">
        <div>
          <div class="project__img">
            <img src="../assets/images/thumbnail1.webp" alt="">
            <span class="image__overlay">
              <div class="project__links">
                <a href="" target="_blank">View Project</a>
                <a href="" target="_blank">View Code</a>
              </div>
            </span>
          </div>
          
        </div>
        
        <div class="project__details">
          <h3>TODO WEB APP</h3>
          <ul class="project__lang">
            <li>Vue-JS</li>
            <li>Vitest</li>
            <li>CSS</li>
          </ul>
        </div>
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
    margin-top: 2rem;
  }

  .projects__title {
    font-size: 5rem;
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

  .projects__cards {
    padding-top: 2rem;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 4rem;
  }

  .project__img {
    width: 34rem;
    height: 28.5rem;
    padding-bottom: 10px;
    position: relative;
  }

  .project__img img {
    width: 100%;
    height: 100%;
    cursor: pointer;
    /* object-fit: contain; */
  }

  h3 {
    font-size: 2rem;
  }

  .project__lang {
    display: flex;
    gap: 1.1rem;
    padding-top: 7px;
  }

  .project__lang li {
    font-size: 1.2rem;
  }

  span.image__overlay {
    background: rgb(36, 36, 36, 0.5);
    width: 34rem;
    height: 28rem;
    position: absolute;
    top: 0;
    right: 0;
    display: none; /*toggle on click" */
  }

  .project__img:hover span.image__overlay {
    display: block;
  }

  .project__links {
    display: flex;
    flex-direction: column;
    background: transparent;
    justify-content: center;
    align-items: center;
    gap: 2rem;
    padding-top: 30%;
  }
</style>