<template>
  <v-app>
    <AppBar />
    <router-view></router-view>
    <!-- <Home /> -->
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import AppBar from "@/components/systemParts/AppBar.vue";
// import Home from "@/views/Home.vue";

export default Vue.extend({
  name: "App",

  components: {
    AppBar
    // Home
  }
});
</script>
