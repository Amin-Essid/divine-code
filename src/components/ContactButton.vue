<template>
  <router-link to="/contact">
    <div :class="buttonClass"><p>CONTACT ME</p></div>
  </router-link>
</template>
<script>
export default {
  name: "ContactButton",
  props: ["buttonClass"],
  setup() {},
};
</script>
<style scoped>
.hero_me_email {
  width: 350px;
  height: 50px;
  color: #f0e68c;
  background: #1b0000;
  font-size: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 5px;
  box-shadow: 2px 2px gray;
  cursor: pointer;
}
.hero_me_email_white {
  width: 350px;
  margin-top: 30px;
  height: 50px;
  color: #1b0000;
  background: white;
  font-size: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 5px;
  box-shadow: 2px 2px gray;
  cursor: pointer;
  margin-bottom: 20px;
}

a {
  text-decoration: none;
}

@media only screen and (max-width: 500px) {
  .hero_me_email {
    width: 100%;
    height: 50px;
    margin-bottom: 20px;
  }
}
</style>
