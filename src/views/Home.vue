<template>
  <v-app light>
    <Header />

    <v-content>
      <Paralogo />

      <MainHome />

      <BackHome />
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import Header from "../components/Header.vue";
import Paralogo from "../components/Paralogo.vue";
import MainHome from "../components/MainHome.vue";
import BackHome from "../components/BackHome.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Home",

  components: { Header, Paralogo, MainHome, BackHome, Footer },
  data() {
    return {};
  },
};
</script>
