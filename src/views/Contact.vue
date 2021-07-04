<template>
  <form @submit.prevent="handleSubmit">
    <!-- text -->
    <p>
      <label>Email:</label>
      <input type="email" v-model="email" required />
    </p>
    <p>
      <label>Message:</label>
      <textarea rows="4" ref="text" type="text" v-model="msg" required />
    </p>
    <div class="submit">
      <button type="submit">CONTACT</button>
    </div>
  </form>
</template>

<script>
// import Hero from "@/components/Hero/Hero.vue";
// import Project from "@/components/Project/Project.vue";
// import InversedProject from "@/components/Project/InversedProject.vue";
// import projects from "@/data/data.js";
// import { ref } from "vue";
export default {
  //   name: "Contact",
  //   props: [],
  //   components: {},
  //   setup() {
  //     // let text = ref(null);
  //     const email = ref("");
  //     const msg = ref("")
  //     // console.log(text);

  //     const handleClick = () => {
  //       console.log(text.value);
  //     };

  //     return { email, handleClick, text };
  //   },

  data() {
    return {
      email: "",
      msg: "",
    };
  },
  methods: {
    handleSubmit() {
      console.log(this.email, this.msg);
    },
  },
};
</script>

<style scoped>
form {
  max-width: 420px;
  margin: 50px auto;
  background: #1b0000;
  text-align: left;
  padding: 40px;
  border-radius: 10px;
}

label {
  color: white;
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 0.6em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}

input {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  color: #555;
}

textarea {
  display: block;
  padding: 10px 6px;
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid #ddd;
  color: #555;
}

button {
  background: white;
  color: #1b0000;
  border: 0;
  padding: 10px 20px;
  margin-top: 20px;
  border-radius: 20px;
  cursor: pointer;
}

.submit {
  text-align: center;
}
</style>
