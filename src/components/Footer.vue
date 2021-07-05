<template>
  <div class="header">
    <div id="nav">
      <!-- <div>
        <router-link to="/">
          <img class="header_logo" alt="logo" src="../assets/logo.png" />
        </router-link>
      </div> -->

      <ContactButton class="hero_me_email" />

      <div class="header_icons">
        <a href="mailto:ameenessid@gmail.com" target="_blank">
          <img class="header_icon" alt="email" src="../assets/email.png" />
        </a>
        <a href="https://github.com/Amin-Essid" target="_blank">
          <img class="header_icon" alt="github" src="../assets/github.png" />
        </a>
        <a
          href="https://www.linkedin.com/in/mohamed-amin-essid-868335143/"
          target="_blank"
        >
          <img
            class="header_icon"
            alt="linkedin"
            src="../assets/linkedin.png"
          />
        </a>
      </div>
    </div>
  </div>
  <router-view />
</template>

<script>
import ContactButton from "@/components/ContactButton.vue";

export default {
  name: "Footer",
  props: [],
  components: { ContactButton },
  setup() {},
};
</script>

<style scoped>
#nav {
  padding: 5px 0;
  margin: 0 auto;
  display: flex;
  width: 80%;
  justify-content: space-between;
  align-items: center;
  margin-top: 10px;
  flex-wrap: wrap;
  /* border-bottom: #1b0000 2px solid; */
}

.header_icon {
  width: 40px;
  height: 40px;
  margin-left: 20px;
  cursor: pointer;
}

@media only screen and (max-width: 500px) {
  #nav {
    width: 95%;
    justify-content: center;
  }
}
</style>
