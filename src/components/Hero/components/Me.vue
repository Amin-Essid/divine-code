<template>
  <div class="hero_me">
    <img class="hero_me_image" src="@/assets/me.png" />
    <!-- <router-link to="/contact">
      <div class="hero_me_email"><p>CONTACT ME</p></div>
    </router-link> -->
    <div class="contact_btn_container">
      <ContactButton buttonClass="hero_me_email" />
    </div>
  </div>
</template>
<script>
import ContactButton from "@/components/ContactButton.vue";
export default {
  name: "Me",
  components: { ContactButton },
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
  border-radius: 5px;
  box-shadow: 2px 2px gray;
  cursor: pointer;
  margin-bottom: 20px;
}

a {
  text-decoration: none;
}

.contact_btn_container {
  margin-bottom: 20px;
  margin-top: 30px;
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
