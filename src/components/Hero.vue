<template>
  <div class="hero">
    <Me />
    <About />
  </div>
</template>

<script>
import About from "@/components/About.vue";
import Me from "@/components/Me.vue";

export default {
  name: "Hero",
  props: [],
  components: { About, Me },
  setup() {},
};
</script>

<style scoped>
.hero {
  display: flex;
  flex-wrap: wrap;
  width: 80%;
  justify-content: space-between;
  align-items: center;
  margin: 50px auto;
}

@media only screen and (max-width: 500px) {
  .hero {
    width: 95%;
  }
}
</style>
