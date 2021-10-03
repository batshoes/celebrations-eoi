<template>
  <img alt="Celebrations Ultra-Premium Collection" src="./assets/Pokemon_TCG_Celebrations_Ultra-Premium_Collection.png">
  <ExpressionsOfInterest msg="Acrylic Display - Expressions of Interest"/>
  <ContactUs />
</template>

<script>
import ExpressionsOfInterest from './components/ExpressionOfInterest.vue'
import ContactUs from './components/ContactUs.vue'

export default {
  name: 'App',
  components: {
    ExpressionsOfInterest,
    ContactUs
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

img {
  width: 70%;
}
</style>
