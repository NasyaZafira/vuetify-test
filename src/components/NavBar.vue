<template>
  <v-app-bar app color="#111111" dark flat class="px-8">
    <v-btn icon>
      <v-icon color="#a69eb0">fa-regular fa-seedling</v-icon>
    </v-btn>

    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')">Home</v-btn>
    <v-btn text @click="scroll('project')">Product</v-btn>
    <v-btn text @click="scroll('about')">About</v-btn>
    <v-btn text @click="scroll('contact')"> contact</v-btn>
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style>
</style>