<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <Demo></Demo>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Demo from "@/components/Demo.vue";

export default {
  name: "Home",
  components: {
    Demo
  }
};
</script>
