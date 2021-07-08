<template>
  <div :class="infoClass">
    <a class="project_info_a" v-if="info.url" :href="info.url" target="_blanc">
      <h2>{{ info.name }}</h2>
      <img src="@/assets/link.png" class="project_info_a_img" />
    </a>

    <h2 v-else>{{ info.name }}</h2>
    <p class="description">{{ info.discreption }}</p>
    <p>
      <span v-for="stuck in info.stucks" :key="stuck">
        {{ stuck }}
      </span>
    </p>
  </div>
</template>

<script>
export default {
  name: "Info",
  props: ["info", "infoClass"],
  components: {},
  setup(props) {
    console.log(props.info);
  },
};
</script>

<style scoped>
.info {
  height: auto;
  width: 550px;
  padding: 0 50px;
  color: #1b0000;
}

.reversedInfo {
  height: auto;
  width: 550px;
  padding: 0 50px;
  color: white;
  /* background: white; */
}

.description {
  text-align: start;
}

.info span {
  display: inline-block;
  color: white;
  background: #1b0000;
  margin: 5px 5px;
  padding: 3px;
  border-radius: 2px;
}

.reversedInfo span {
  display: inline-block;
  color: #1b0000;
  background: white;
  margin: 5px 5px;
  padding: 3px;
  border-radius: 2px;
}

.project_info_a {
  text-decoration: none;
  color: inherit;
}

.project_info_a_img {
  width: 20px;
  height: auto;
  margin-left: 5px;
}

h2 {
  display: inline-block;
}

p {
  text-align: start;
}
@media only screen and (max-width: 500px) {
  .info,
  .reversedInfo {
    width: 95%;
  }
}
</style>
