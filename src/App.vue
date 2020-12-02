<template>
  <v-app>
    <v-app-bar app color="" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>
    </v-app-bar>

    <v-main>
      <TablaCuenta></TablaCuenta>
      <TablaCuentahabiente></TablaCuentahabiente>
      <Footer></Footer>
    </v-main>
  </v-app>
</template>

<script>
import TablaCuenta from "./components/TablaCuenta";
import TablaCuentahabiente from "./components/TablaCuentahabiente";
import Footer from "./components/Footer";

export default {
  name: "App",

  components: {
    Footer,
    TablaCuenta,
    TablaCuentahabiente
  },

  data: () => ({
    //
  })
};
</script>
