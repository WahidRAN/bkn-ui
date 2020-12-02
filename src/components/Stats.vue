<template>
  <section id="stats">
    <v-parallax
      :height="$vuetify.breakpoint.smAndDown ? 700 : 500"
      src="https://images.unsplash.com/photo-1510915228340-29c85a43dcfe?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80"
    >
      <v-container fill-height>
        <v-row class="mx-auto">
          <v-col v-for="[value, title] of stats" :key="title" cols="12" md="3">
            <div class="text-center">
              <div
                class="display-3 font-weight-black mb-4"
                v-text="value"
              ></div>

              <div
                class="title font-weight-regular text-uppercase"
                v-text="title"
              ></div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-parallax>
  </section>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "Stats",
  data() {
    return {
      stats: [
        ["316", "Pengunjung Hari ini"],
        ["17361", "Pengunjung Bulan ini"],
        ["253397", "Pengunjung Tahun ini"],
        ["253397", "Total Pengunjung"]
      ]
    };
  }
});
</script>
