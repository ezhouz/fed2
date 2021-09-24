<template>
  <section>
    <Navbar class="nested-navbar" />
    <Body />
  </section>
</template>

<script>
import Body from "./Body.vue";
import Navbar from "./Navbar.vue";

export default {
  name: "Home",
  components: {
    Body,
    Navbar,
  },
};
</script>

<style scoped>
</style>