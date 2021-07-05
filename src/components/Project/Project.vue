<template>
  <div class="project">
    <Preview :preview="project.preview" previewClass="preview" />
    <Info :info="project.info" infoClass="info" />
  </div>

  <div class="contact_btn_container">
    <ContactButton class="hero_me_email " />
  </div>
</template>

<script>
import Preview from "@/components/Project/components/Preview.vue";
import Info from "@/components/Project/components/Info.vue";
import ContactButton from "@/components/ContactButton.vue";

export default {
  name: "Project",
  props: ["project"],
  components: { Preview, Info, ContactButton },
  setup() {},
};
</script>

<style scoped>
.project {
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  padding-top: 175px;
  padding-bottom: 175px;

  /* border-bottom: #1b0000 2px solid; */
}

.contact_btn_container {
  margin: 0 0 100px 0;
  display: flex;
  justify-content: center;
}
/* @media only screen and (max-width: 500px) {

} */
</style>
