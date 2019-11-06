<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Email id="email" />
  </div>
</template>

<script>
import Email from "./components/Email.vue";

export default {
  name: "app",
  components: {
    Email
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#email {
  width: 50%;
  margin: 0 auto;
}
</style>
