<template>
  <v-app>
    <AppBar />

    <v-content>
      <Hero />
      <About />
      <Berita />
      <Layanan />
      <Stats />
      <Kontak />
      <Footer />
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue"; // @ is an alias to /src
import About from "@/components/About.vue";
import AppBar from "@/components/AppBar.vue";
import Berita from "@/components/Berita.vue";
import Footer from "@/components/Footer.vue";
import Hero from "@/components/Hero.vue";
import Kontak from "@/components/Kontak.vue";
import Layanan from "@/components/Layanan.vue";
import Stats from "@/components/Stats.vue";
// import HelloWorld from "@/components/HelloWorld.vue";

export default Vue.extend({
  name: "Home",
  components: {
    About,
    AppBar,
    Berita,
    Footer,
    Hero,
    Kontak,
    Layanan,
    Stats
    // HelloWorld
  }
});
</script>
