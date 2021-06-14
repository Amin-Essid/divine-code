<template>
  <div :class="previewClass">
    <img
      class="previewImage"
      :src="require('@/assets/projects/' + preview[0] + '')"
    />
  </div>
</template>

<script>
export default {
  name: "Preview",
  props: ["preview", "previewClass"],
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

.previewImage {
  height: 440px;
  width: 550px;
}

.reversedPreview {
  height: 440px;
  width: 550px;
  background: white;
}
/* @media only screen and (max-width: 500px) {

} */
</style>
