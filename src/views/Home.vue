<template>
  <div class="home">
    <Hero />
    <div class="title">
      <h1>
        MY WORK
      </h1>
    </div>
    <!-- <div
      v-for="project in projects"
      :key="project.id"
      class="projects"
      :id="project.info.name"
    > -->
    <InversedProject :project="projects[0]" />
    <Project :project="projects[1]" />
    <InversedProject :project="projects[2]" />
    <Project :project="projects[3]" />
    <InversedProject :project="projects[4]" />
    <!-- </div> -->
  </div>

  <Footer />
</template>

<script>
import Hero from "@/components/Hero/Hero.vue";
import Project from "@/components/Project/Project.vue";
import InversedProject from "@/components/Project/InversedProject.vue";
import projects from "@/data/data.js";
import Footer from "@/components/Footer.vue";
export default {
  name: "Home",
  props: [],
  components: { Hero, Project, InversedProject, Footer },
  setup() {
    return { projects };
  },
};
</script>

<style scoped>
.title {
  margin-bottom: 30px;
  color: #1b0000;
  margin-top: 30px;
}

.title h1 {
  display: inline-block;
  padding-bottom: 10px;
  border-bottom: #1b0000 2px solid;
}
</style>
