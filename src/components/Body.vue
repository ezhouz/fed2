<template>
  <div>
    <div>
      <hr class="red-line" />
    </div>

    <section class="text-section">
      <article class="page-text">
        <h1>
          Sed fermentum tortor vitae justo rhoncus, vitae ultricies ante
          ultricies.
        </h1>

        <p>
          Fusce ultricies sit amet diam sit amet pulvinar. Vivamus id augue
          neque. Praesent massa magna, tempor vel blandit id, volutpat eu orci.
          Pellentesque varius eros sed tempus pre.
        </p>
      </article>
    </section>
  </div>
</template>

<script>
export default {
  name: "Body",
  components: {},
};
</script>

<style scoped>
.red-line {
  width: 10%;
  border-top: 2px solid #c02d2d;
  margin: 9rem auto 4rem auto;
}
.text-section {
  font-family: Helvetica, sans-serif;
  letter-spacing: 0;
  text-align: center;
  width: 70%;
  margin: 0 auto;
}
h1 {
  font-size: 4.5rem;
  color: #9b9b9b;
}
p {
  color: #dfdfdf;
  font-size: 2.5rem;
  margin: 0 auto 20rem auto
}
</style>
