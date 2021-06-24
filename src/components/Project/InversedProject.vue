<template>
  <div class="project">
    <Info :info="project.info" infoClass="reversedInfo" />
    <Preview :preview="project.preview" previewClass="reversedPreview" />
  </div>
</template>

<script>
import Preview from "@/components/Project/components/Preview.vue";
import Info from "@/components/Project/components/Info.vue";

export default {
  name: "InversedProject",
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
  flex-wrap: wrap-reverse;
  padding-top: 175px;
  padding-bottom: 175px;
  background: #1b0000;

  /* border-bottom: #1b0000 2px solid; */
}
/* @media only screen and (max-width: 500px) {

} */
</style>
