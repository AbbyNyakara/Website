<template>
  <div class="contact">
    <div class="contact__description">
      <h2>Contact</h2>
      <p>I would love to hear about your project and how I 
        can make it come alive! Please fill in the form and 
        i'll get back to you as soon as possible
      </p>
    </div>
    <form action="" class="contact__form">
      <input v-model="text" name="name" placeholder="NAME" required>
      <input v-model="email" name="email" placeholder="EMAIL" required>
      <textarea v-model="message" name="message" required cols="30" rows="5" placeholder="MESSAGE"></textarea>
      <button type="submit" class="send__button">SEND MESSAGE</button>
    </form>
  </div>
</template>

<script>
  import emailjs from 'emailjs-com';

  export default {
    name: "Contact"
  }
</script>

<style scoped>
  .contact {
    margin-top: 7rem;
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
    width: 80%;
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
    margin-bottom: 2rem;
    border-bottom: 2px solid grey;
    color: #fff;
    padding-bottom: 1.2rem;
    font-size: 1.1rem;
    resize: none;
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