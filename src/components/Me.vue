<template>
  <div class="hero_me">
    <img class="hero_me_image" src="../assets/me.jpg" />
    <div class="hero_me_email"><p>ameenessid@gmail.com</p></div>
  </div>
</template>
<script>
export default {
  name: "Me",
  setup() {},
};
</script>
<style scoped>
.hero_me_image {
  width: 350px;
  height: 350px;
}
.hero_me_email {
  width: 350px;
  margin-top: 30px;
  height: 50px;
  color: #f0e68c;
  background: #1b0000;
  font-size: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
}

@media only screen and (max-width: 500px) {
  .hero_me_image {
    width: 95%;
    height: auto;
  }
  .hero_me_email {
    width: 100%;
    height: 50px;
    margin-bottom: 20px;
  }
}
</style>
