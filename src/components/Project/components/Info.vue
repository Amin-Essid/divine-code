<template>
  <div :class="infoClass">
    <h2>{{ info.name }}</h2>
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
