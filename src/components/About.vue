<template>
  <section id="about-me">
    <div class="py-8"></div>

    <v-container>
      <v-row>
        <v-col class="text-center" cols="12" md="6">
          <v-img height="450px" src="@/assets/1.png" contain></v-img>
          <v-img height="200px" src="@/assets/2.jpg" contain></v-img>
          <v-img height="200px" src="@/assets/3.jpg" contain></v-img>
        </v-col>
        <v-col cols="12" md="6">
          <h2 class="display-2 font-weight-bold mb-3 text-center">AGENDA</h2>
          <v-timeline :dense="$vuetify.breakpoint.smAndDown">
            <v-timeline-item v-for="({ date, text }, i) in agendas" :key="i">
              <span class="headline" slot="opposite" v-text="date"></span>
              <v-card class="elevation-2">
                <v-card-text v-text="text"></v-card-text>
              </v-card>
            </v-timeline-item>
          </v-timeline>
          <v-row>
            <v-spacer></v-spacer>
            <v-btn class="mt-16" color="primary">Agenda Lainnya</v-btn>
            <v-spacer></v-spacer>
          </v-row>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12" md="4">
          <v-img height="200px" src="@/assets/statuskp.jpg" contain></v-img>
        </v-col>
        <v-col cols="12" md="4">
          <v-img height="200px" src="@/assets/statuspen.jpg" contain></v-img>
        </v-col>
        <v-col cols="12" md="4">
          <v-img
            height="200px"
            src="@/assets/eworkshopcorel.jpg"
            contain
          ></v-img>
        </v-col>
      </v-row>
    </v-container>

    <div class="py-0"></div>
  </section>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "About",
  data: () => ({
    agendas: [
      {
        date: "1-28 September 2020",
        text:
          "Pelaksanaan Seleksi Kompetensi Bidang (SKB) CPNS Formasi Tahun 2019 di Titik Lokasi Wilayah Kerja Kantor Regional V BKN Jakarta"
      },
      {
        date: "3-5 September 2019",
        text:
          "Penilaian Potensi dan Kompetensi bagi Pejabat Pimpinan Tinggi Pratama dan Administrator (Talent Pool) di UPT BKN Pontianak"
      },
      {
        date: "1-2 Agustus 2019",
        text:
          "Workshop Pengelolaan Kepegawaian Berbasis Merit di Pusat Pengembangan ASN Ciawi"
      },
      {
        date: "29-30 Juli 2019",
        text:
          "Workshop Pengukuran Indeks Profesionalitas ASN oleh Direktorat Jabatan ASN di Hotel Ciputra Jakarta"
      }
    ]
  })
});
</script>
