<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <!-- <Home /> -->
    <Home2 />
  </div>
</template>

<script>
// import Home from "./components/Home.vue";
import Home2 from "./components/Home2.vue";

export default {
  name: "App",
  components: {
    // Home,
    Home2,
  },
};
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
</style>
