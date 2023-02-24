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
      <div class="project__card" v-for="(project, index) in projects" :key="index">
        <div>
          <div class="project__img">
              <!-- Project image not working in deployment -->
            <img :src="project.img" alt="">
            <span class="image__overlay">
              <div class="project__links">
                <!-- Add the links here -->
                <a :href="project.live" target="_blank">View Project</a>
                <a :href="project.code" target="_blank">View Code</a>
              </div>
            </span>
          </div>
        </div>
        
        <div class="project__details">
          <h3>{{project.name}}</h3>
          <div class="techs_used">
            <ul class="project__lang" v-for="(tech, index) in project.techs" :key="index"> 
              <li>{{tech}}</li>
            </ul>
          </div>
        </div>
      </div>
      <!-- End -->
    </div>
  </div>
</template>

<script>
  export default {
    name: "Projects",
    data() {
      return {
        projects: [
          {
            name: "Doctor Appointment Booking App",
            techs: ["Rails", "React", "SCSS"],
            img: "/doctor.png",
            live: "https://doc-appointments.netlify.app/",
            code: "https://github.com/TracK92/doctor-appointment-front-end"
          },
          {
            name: "Smile Essence Dental Website",
            techs: ["React", "TailwindCSS"],
            img: "/smile.png",
            live: "https://smile-essence.vercel.app/",
          },
          {
            name: "Waymark Dental Website",
            techs: ["React", "SEO", "SCSS"],
            img: "/waymark.webp",
            live: "https://dental-website.vercel.app/",
            code: "https://github.com/AbbyNyakara/DentalWebsite"
          },
          {
            name: "Space Traveller's Hub",
            techs: ["React", "Redux", "Jest", "API"],
            img: "/space.webp",
            live: "https://extraordinary-blini-9b9ffd.netlify.app/",
            code: "https://github.com/AbbyNyakara/spaceship-project"
          },
          {
            name: "Designo Website",
            techs: ["React", "SCSS", "Jest", "React Router"],
            img: "/designo.png",
            live: "https://designo-website-phi.vercel.app/",
            code: "https://github.com/AbbyNyakara/Designo-Website"
          },
          {
            name: "Todo web App",
            techs: ["VueJS", "Vitest", "CSS"],
            img: "/todo.webp",
            live: "https://todo-list-vue-submission.vercel.app/",
            code: "https://github.com/AbbyNyakara/TodoListVueSubmission"
          },
        ]
      }
    }
  }
</script>

<style scoped>
  .projects {
    margin-top: 4rem;
    border-top: 2px solid grey;
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
    height: 20.5rem;
    position: relative;
  }

  .project__img img {
    width: 100%;
    height: 100%;
    cursor: pointer;
    object-fit: cover;
    padding-bottom: 1rem;
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
    height: 21rem;
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
    padding-top: 20%;
  }

  .techs_used {
    display: flex;
    gap: 1rem;
  }

  @media only screen and (max-width: 960px) {
    .projects__title {
      font-size: 2rem;
    }

    .projects__cards {
      grid-template-columns: 1fr;
    }

    .project__img {
      width: 100%;
      height: 100%;
    }

    span.image__overlay {
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      right: 0;
      display: none; /*toggle on click" */
    }
  }
</style>
