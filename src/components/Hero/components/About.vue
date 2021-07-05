<template>
  <div class="hero_about">
    <p class="hero_about_one">
      Hi, I am Amine Essid.
    </p>
    <p>
      I am a passionate software developer and a teacher, I have been working on
      multiple challenging projects for the past few years as a consultant and
      freelancer.
    </p>
    <p>My favourite tecknologies are React js, Vue js and Node js.</p>
    <p>
      Finally my dream is to build a platform that supports children education
      in Africa, and I am open to all the opportunities that can extend my
      expertise, my knowledge, and my competence in order to achieve that dream.
    </p>
  </div>
</template>

<script>
export default {
  name: "About",
  setup() {},
};
</script>

<style scoped>
.hero_about {
  max-width: 750px;
  width: 100%;
  min-height: 420px;
  height: auto;
  color: white;
  background: #1b0000;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  font-size: 20px;
  padding: 10px;
}

.hero_about p {
  text-align: left;
  margin-top: 15px;
}
/* .hero_about_one {
  padding-left: 15px;
} */
</style>
