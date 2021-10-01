<template>
  <img alt="Celebrations Ultra-Premium Collection" src="./assets/Pokemon_TCG_Celebrations_Ultra-Premium_Collection.png">
  <ExpressionsOfInterest msg="Acrylic Display - Expressions of Interest"/>
</template>

<script>
import ExpressionsOfInterest from './components/ExpressionOfInterest.vue'

export default {
  name: 'App',
  components: {
    ExpressionsOfInterest
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
