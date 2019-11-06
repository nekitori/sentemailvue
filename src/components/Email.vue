<template>
  <form class="contact-form" @submit.prevent="sendEmail">
    <label>De</label>
    <input type="text" name="from_name" />
    <label>Para</label>
    <input type="text" name="name" />
    <label>Email</label>
    <input type="text" name="email" />
    <label>mensaje</label>
    <textarea name="mensaje"></textarea>
    <input type="submit" value="Send" />
  </form>
</template>

<script>
import emailjs from "emailjs-com";

export default {
  methods: {
    sendEmail: e => {
      emailjs.sendForm(
        "gmail",
        "template_oZeeUwJr",
        e.target,
        "user_FoEH1tHInAzbaonBdRlO1"
      );
    }
  }
};
</script>