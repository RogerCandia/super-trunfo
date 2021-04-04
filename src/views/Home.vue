<template>
  <div class="home">
    <img alt="Vue logo" :src="imageSource" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <button @click="changeImageSource('cassius')">clique</button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import VueImage from "../assets/logo.png";

export default {
  name: "Home",
  data() {
    return {
      imageSource: VueImage,
    };
  },
  components: {
    HelloWorld,
  },
  methods: {
    changeImageSource(url) {
      this.imageSource = url;
    },
  },
};
</script>
