<template>
  <div class="info"></div>
</template>

<script>
export default {
  name: "Info",
  props: ["info"],
  components: {},
  setup(props) {
    console.log(props.info);
  },
};
</script>

<style scoped>
.info {
  height: 440px;
  width: 650px;
  background: #1b0000;
}
/* @media only screen and (max-width: 500px) {

} */
</style>
