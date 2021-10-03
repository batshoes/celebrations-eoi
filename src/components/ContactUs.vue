<template>
  <form ref="form" @submit.prevent="sendEmail">
    <label>Name</label>
    <input type="text" name="user_name">
    <label>Email</label>
    <input type="email" name="user_email">
    <label>Message</label>
    <textarea name="message"></textarea>
    <input type="submit" value="Send">
  </form>
</template>

<script>
import emailjs from 'emailjs-com';
console.log(process.env.VUE_APP_ENV_TEST)
console.log(process.env.VUE_APP_EOI_EMAIL_JS_USER_ID)
console.log(process.env.VUE_APP_EOI_EMAIL_TEMPLATE_ID)
console.log(process.env.VUE_APP_EOI_EMAIL_SERVICE_ID)
export default {
  methods: {
    sendEmail() {
      emailjs.sendForm(process.env.VUE_APP_EOI_EMAIL_SERVICE_ID, process.env.VUE_APP_EOI_EMAIL_TEMPLATE_ID, this.$refs.form, process.env.VUE_APP_EOI_EMAIL_JS_USER_ID)
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        });
    }
  }
}
</script>