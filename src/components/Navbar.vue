<template>
  <div class="navbar-container">
    <nav>
      <ul class="navbar-list">
        <li
          class="navbar-list__item"
          v-for="(navitem, index) in navitems"
          :key="index"
          :class="{ active: activeIndex === index }"
          @click="setActive(index)"
        >
          {{ navitem.name }}
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data: function () {
    return {
      navitems: [{ name: "Item 1" }, { name: "Item 2" }, { name: "Item 3" }],
      activeIndex: 0,
    };
  },
  methods: {
    setActive(index) {
      this.activeIndex = index;
    },
  },
};
</script>

<style scoped>
.navbar-container {
  background: url("../../public/images/shoes.png");
  height: 45rem;
  background-position: -20rem 49rem;
  background-size: 152rem;
  position: relative;
}
nav {
  position: absolute;
  bottom: 0;
  width: 100%;
}
.navbar-list {
  width: 100%;
  display: flex;
  background: #9b9b9b;
  opacity: 0.5;
  list-style-type: none;
  margin: 0;
  padding: 0;
}
.navbar-list__item {
  height: 5rem;
  width: 20rem;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 1.6rem;
  cursor: pointer;
}
.navbar-list__item.active {
  background: #fff;
}
</style>