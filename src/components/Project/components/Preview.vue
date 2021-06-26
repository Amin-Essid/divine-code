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
  height: 310px;
  width: 550px;
  border: #1b0000 solid 2px;
}

.previewImage {
  height: auto;
  width: 550px;
}

.reversedPreview {
  height: 310px;
  width: 550px;
  border: white solid 2px;
}
@media only screen and (max-width: 500px) {
  .preview,
  .reversedPreview {
    width: 95%;
    margin-bottom: 20px;
  }

  .previewImage {
    width: 80%;
  }
}
</style>
