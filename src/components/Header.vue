<template>
  <div class="header">
    <div id="nav">
      <div>
        <router-link to="/">
          <img class="header_logo" alt="logo" src="../assets/logo.png" />
        </router-link>
      </div>

      <div class="header_icons">
        <a href="#">
          <img class="header_icon" alt="facebook" src="../assets/fb.png" />
        </a>
        <a href="#">
          <img
            class="header_icon"
            alt="instagram"
            src="../assets/instagram.png"
          />
        </a>
        <a href="#">
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
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: "Header",
  props: [],
  components: {},
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
  border-bottom: #1b0000 2px solid;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.header_logo {
  width: 50px;
  height: 50px;
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
  }
}
</style>
