<template>
  <div class="skills">
    <div class="skills__cards">
      <div id="skill__names">
       ✧ HTML ✧ CSS ✧ JavaScript ✧ SASS ✧ ReactJS ✧ VueJS ✧ Redux ✧ SQL ✧ Ruby ✧ Ruby On Rails ✧ Jest ✧ Vitest ✧Python
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Skills",
    mounted () {
      // const text = document.getElementById('skill__names');
      // text.innerHTML = text.textContent.replace(/\S/g, "<span>$&</span>");
      // const ele = document.querySelectorAll('span');
      // for (let i=0; i<ele.length; i++) {
      //   ele[i].style.transform="rotate("+i*360/ele.length+"deg)"
      // }
    } 
  }

</script>

<style scoped>
  .skills {
    margin-top: 4rem;
    width: 100%;
    margin-bottom: 3rem;
    padding-top: 3rem;
  }

  span {
    position: absolute;
    transform-origin: 0 80px;
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
