<template>
  <div class="contact">
    <div class="contact__description">
      <h2>Contact</h2>
      <p>I would love to hear about your project and how <br> I 
        can make it come alive! Please fill in the form and <br>
        i'll get back to you as soon as possible
      </p>
    </div>
    <form action="" class="contact__form">
      <input type="text" placeholder="NAME">
      <input type="email" name="" id="" placeholder="EMAIL">
      <textarea name="" id="" cols="30" rows="5" placeholder="MESSAGE"></textarea>
      <button class="send__button">SEND MESSAGE</button>
    </form>
  </div>
</template>

<script>
  export default {
    name: "Contact"
  }
</script>

<style scoped>
  .contact {
    position: relative;
    top: 340vh; /*This will not work*/
    display: flex;
    gap: 3rem;
    justify-content: space-between;
    align-items: center;
    min-height: 80vh;
    padding-bottom: 2rem;
    border-bottom: 2px solid #fff;
    /* background-color: rgb(78, 76, 76) */
  }

  .contact__description {
    flex: 1.1;
  }

  .contact__description p {
    line-height: 1.5;
    font-size: 1.1rem;
    padding-top: 1.2rem;
  }

  .contact h2 {
    font-size: 5rem;
  }

  .contact__form {
    display: grid;
    flex: 0.9;
  }

  input,
  textarea {
    border: none;
    outline: none;
    margin-bottom: 5rem;
    border-bottom: 2px solid grey;
    color: #fff;
    padding-bottom: 1.2rem;
    font-size: 1.1rem;
  }

  .send__button {
    border: none;
    font-size: 1.1rem;
    color: #fff;
    margin-left: auto;
    border-bottom: 2px solid rgb(78, 225, 160);
    padding-bottom: 1.1rem;
  }

  input::placeholder,
  textarea::placeholder {
    color: rgb(78, 76, 76);
    font-size: 1.1rem;
  }
</style>