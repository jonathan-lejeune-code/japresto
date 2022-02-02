<template>
  <v-app light>
    <Header />

    <v-content>
      <Paralogo />
      <MainContact />
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import Header from "../components/Header.vue";
import Paralogo from "../components/Paralogo.vue";
import MainContact from "../components/mainContact.vue";

import Footer from "../components/Footer.vue";
export default {
  components: { Header, Paralogo, MainContact, Footer },
};
</script>

<style></style>
