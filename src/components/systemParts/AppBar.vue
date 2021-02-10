<template>
  <v-app-bar app dense color="primary" height="70">
    <v-avatar class="mr-3" color="primary" size="70">
      <v-img contain max-height="100%" src="@/assets/logo.png"></v-img>
    </v-avatar>
    <v-spacer></v-spacer>
    <v-tabs right color="white">
      <v-tab :to="'/'" @click="$vuetify.goTo('#hero')">Beranda</v-tab>
      <v-tab :to="'/profil'">Profil</v-tab>
      <v-tab @click="$vuetify.goTo('#berita')">Berita</v-tab>
      <v-tab @click="$vuetify.goTo('#layanan')">Layanan</v-tab>
      <v-tab @click="$vuetify.goTo('#contact')">Kontak</v-tab>
      <!-- <v-tab>Galeri</v-tab>
      <v-tab>Pertanyaan Umum</v-tab> -->
    </v-tabs>
  </v-app-bar>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "AppBar"
});
</script>
