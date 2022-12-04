<template>
  <div class="skills">
    <div class="skills__cards">
      <div class="skills__card" v-for="(skill, index) in skills" :key="index">
        <div class="skills__card-title">{{skill.title}}</div>
        <div class="skills__card-years">{{skill.experience}}</div>
      </div>
    </div>
    <img src="../assets/images/pattern-rings.svg" class="rings__skills" alt="">
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
    position: absolute;
    top: 100vh;
    border-top: 2px solid grey;
    width: 80%;
    padding-top: 3rem;
    margin-bottom: 3rem;
    height: 100vh;
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

  .skills__cards::after {
    background: url(../assets/images/pattern-rings.svg);
    content: "";
  }

  .rings__skills {
    position: absolute;
    top: 75vh;
    right: -40%;
    z-index: 20;
  }
</style>