<template>
  <div class="home">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <router-link to="/about">About</router-link>
    <div>{{ mount }}</div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "HomeView",
  components: {
    // HelloWorld,
  },
  data: function () {
    return {
      mount: "",
    };
  },
  created: function () {
    const a = "111";
    this.mount = this.utils.li(a);
  },
};
</script>
