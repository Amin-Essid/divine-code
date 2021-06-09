<template>
  <div class="project">
    <Preview :preview="project.preview" />
    <Info :info="project.info" />
  </div>
</template>

<script>
import Preview from "@/components/Project/components/Preview.vue";
import Info from "@/components/Project/components/Info.vue";

export default {
  name: "Project",
  props: ["project"],
  components: { Preview, Info },
  setup() {},
};
</script>

<style scoped>
.project {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 50px;
  margin-bottom: 200px;
  /* border-bottom: #1b0000 2px solid; */
}
/* @media only screen and (max-width: 500px) {

} */
</style>
