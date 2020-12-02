<template>
  <section id="hero">
    <v-row no-gutters>
      <v-img src="../assets/hero.jpg">
        <v-theme-provider dark>
          <v-container fill-height>
            <v-row align="center" class="white--text mx-auto" justify="center">
              <v-col class="primary--text text-center" cols="12" tag="h1">
                <span
                  :class="[
                    $vuetify.breakpoint.smAndDown ? 'display-1' : 'display-2'
                  ]"
                  class="font-weight-light"
                >
                  Kantor Regional V
                </span>

                <br />

                <span
                  :class="[
                    $vuetify.breakpoint.smAndDown ? 'display-3' : 'display-4'
                  ]"
                  class="font-weight-black"
                >
                  BKN Jakarta
                </span>
              </v-col>

              <v-btn
                class="align-self-end"
                color="black"
                fab
                outlined
                @click="$vuetify.goTo('#about-me')"
              >
                <v-icon>mdi-chevron-double-down</v-icon>
              </v-btn>
            </v-row>
          </v-container>
        </v-theme-provider>
      </v-img>
    </v-row>
  </section>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "Hero"
});
</script>
