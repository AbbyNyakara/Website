<template>
  <div class="contact">
    <div class="contact__description">
      <h2>Contact</h2>
      <p>I would love to hear about your project and how I 
        can make it come alive! Please fill in the form and 
        i'll get back to you as soon as possible
      </p>
    </div>
    <form ref="form" action="" class="contact__form" @submit.prevent="sendEmail()">
      <input name="name" placeholder="NAME" required>
      <input name="email" placeholder="EMAIL" required>
      <textarea name="message" required cols="30" rows="5" placeholder="MESSAGE"></textarea>
      <button type="submit" class="send__button" value="send" >SEND MESSAGE</button>
    </form>
  </div>
</template>

<script>
  import emailjs from 'emailjs-com';

  export default {
    name: "Contact",
    data() {
      return {
        name: '',
        email: '',
        message: ''
      }
    },
    methods: {
      sendEmail() {
        emailjs.sendForm('Abby2020#', 'template_jypst7o', this.$refs.form , 'fsohKjm6d5QCqbnm7')
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        });
        this.name = ''
        this.email = ''
        this.message = ''
      },
    }
  }
</script>

<style scoped>
  .contact {
    margin-top: 5rem;
    display: flex;
    gap: 3rem;
    justify-content: space-between;
    align-items: center;
    min-height: 80vh;
    padding-bottom: 2rem;
    border-bottom: 2px solid #fff;
    /* background-color: hsl(0, 0%, 14%); */
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

  @media only screen and (max-width: 960px) {
    .contact {
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .contact h2 {
      font-size: 2.5rem;
      text-align: center;
    }

    .contact__description p {
      text-align: center;
      margin: auto;
    }
  }
</style>