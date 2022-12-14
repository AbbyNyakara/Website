<template>
  <div class="skills">
    <div class="skills__cards">
      <div class="skills__card" v-for="(skill, index) in skills" :key="index">
        <div class="skills__card-title">{{skill.title}}</div>
        <div class="skills__card-years">{{skill.experience}}</div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Skills",
    data() {
      return {
        skills: [
          {
            title: "JavaScript",
            experience: "2 Years Experience",
          },
          {
            title: "SASS",
            experience: "1 Year Experience",
          },
          {
            title: "React",
            experience: "1 Year Experience",
          },
          {
            title: "Redux",
            experience: "1 Year Experience",
          },
          {
            title: "Vue-JS",
            experience: "1 Year Experience",
          },
          {
            title: "Ruby",
            experience: "1 Year Experience",
          },
          {
            title: "Rails",
            experience: "1 Year Experience",
          },
          {
            title: "Python",
            experience: "1 Year Experience",
          },
          {
            title: "Accesibility",
            experience: "1 Year Experience",
          },
          {
            title: "Jest & Vitest",
            experience: "1 Year Experience",
          },
          {
            title: "PostgreSQL",
            experience: "1 Year Experience",
          },
          {
            title: "MySQL",
            experience: "1 Year Experience",
          },
          {
            title: "HTML",
            experience: "1 Year Experience",
          },
          {
            title: "CSS",
            experience: "1 Year Experience",
          },
        ]
      }
    }
  }
</script>

<style scoped>
  .skills {
    margin-top: 4rem;
    border-top: 2px solid grey;
    width: 100%;
    margin-bottom: 3rem;
    min-height: 100vh;
    padding-top: 3rem;
  }

  .skills__card-title {
    font-weight: bolder;
    font-size: 2.3rem;
  }

  .skills__cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-row-gap: 4rem;
  }

  .rings__skills {
    position: absolute;
    top: 75vh;
    right: -40%;
    z-index: 20;
  }

  @media only screen and (max-width: 960px) {
    .skills {
      margin-top: 0.5rem;
    }

    .skills__card-title {
      font-size: 1.5rem;
    }

    .skills__cards {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media only screen and (max-width: 400px) {
     .skills__cards {
      grid-template-columns: 1fr;
      place-items: center;
    }
  }
</style>