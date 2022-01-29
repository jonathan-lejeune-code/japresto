<template>
  <v-app light>
    <Header />

    <v-content>
      <Paralogo />

      <MenuCard />
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import Header from "../components/Header.vue";
import Paralogo from "../components/Paralogo.vue";
import MenuCard from "../components/MenuCard.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Menu",

  components: { Header, Paralogo, MenuCard, Footer },
  data() {
    return {};
  },
};
</script>
