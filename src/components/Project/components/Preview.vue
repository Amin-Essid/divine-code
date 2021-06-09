<template>
  <div class="preview">
    <!-- <img :src="preview[0]" /> -->
  </div>
</template>

<script>
export default {
  name: "Preview",
  props: ["preview"],
  components: {},
  setup(props) {
    console.log(props.preview);
  },
};
</script>

<style scoped>
.preview {
  height: 440px;
  width: 550px;
  background: #1b0000;
}
/* @media only screen and (max-width: 500px) {

} */
</style>
