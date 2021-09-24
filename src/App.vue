<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from "./components/Home.vue";

export default {
  name: "App",
  components: {
    Home,
  },
};
</script>

<style>
html, body {
  font-size: 62.7%;
}
#app {
  margin: 0 auto;
  max-width: 1280px;
}
</style>
