<template>
  <v-main>
    <Hero />
    <About />
    <Berita />
    <Layanan />
    <Stats />
    <Kontak />
    <Footer />
  </v-main>
</template>

<script lang="ts">
import Vue from "vue"; // @ is an alias to /src
import About from "@/components/About.vue";
import Berita from "@/components/Berita.vue";
import Footer from "@/components/Footer.vue";
import Hero from "@/components/Hero.vue";
import Kontak from "@/components/Kontak.vue";
import Layanan from "@/components/Layanan.vue";
import Stats from "@/components/Stats.vue";

export default Vue.extend({
  name: "Home",
  components: {
    About,
    Berita,
    Footer,
    Hero,
    Kontak,
    Layanan,
    Stats
  }
});
</script>
