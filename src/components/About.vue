<template>
  <section id="about-me">
    <div class="py-12"></div>

    <v-container class="text-center">
      <h2 class="display-2 font-weight-bold mb-3">VISI</h2>

      <v-responsive class="mx-auto mb-8" width="56">
        <v-divider class="mb-1"></v-divider>

        <v-divider></v-divider>
      </v-responsive>

      <v-responsive
        class="mx-auto title font-weight-light mb-8"
        max-width="720"
      >
        “Menjadi Pembina dan Penyelenggara Manajemen Kepegawaian yang
        Profesional dan Bermartabat Tahun 2025”
      </v-responsive>

      <!-- <v-avatar class="elevation-12 mb-12" size="128">
        <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
      </v-avatar>

      <div></div>

      <v-btn color="grey" href="https://vuetifyjs.com" outlined large>
        <span class="grey--text text--darken-1 font-weight-bold">
          Vuetify Documentation
        </span>
      </v-btn> -->
    </v-container>
    <v-container class="text-center">
      <h2 class="display-2 font-weight-bold mb-3">MISI</h2>

      <v-responsive class="mx-auto mb-8" width="56">
        <v-divider class="mb-1"></v-divider>

        <v-divider></v-divider>
      </v-responsive>

      <v-responsive
        class="mx-auto title font-weight-light mb-8"
        max-width="720"
      >
        <v-row>
          <v-col class="mx-2"
            >Mengembangkan Sistem Manajemen Kepegawaian Negara</v-col
          >
          <v-col class="mx-2">Mengembangkan Sistem Pelayanan Kepegawaian</v-col>
          <v-col class="mx-2">Mengembangkan Manajemen Internal BKN</v-col>
        </v-row>
      </v-responsive>

      <!-- <v-avatar class="elevation-12 mb-12" size="128">
        <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
      </v-avatar>

      <div></div>

      <v-btn color="grey" href="https://vuetifyjs.com" outlined large>
        <span class="grey--text text--darken-1 font-weight-bold">
          Vuetify Documentation
        </span>
      </v-btn> -->
    </v-container>

    <div class="py-12"></div>
  </section>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "About"
});
</script>
