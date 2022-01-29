<template>
  <v-app-bar>
    <v-toolbar color="#FFF4E0" app>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn
          flat
          text
          color="red"
          v-for="item in menuItems"
          :key="item.title"
          :to="item.path"
        >
          <v-icon left dark>{{ item.icon }}</v-icon>
          {{ item.title }}
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </v-app-bar>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      sidebar: false,
      menuItems: [
        { title: "Home", path: "/", icon: "mdi-home" },
        { title: "Menu", path: "/menu", icon: "mdi-book-open-variant" },
        { title: "Contact", path: "/contact", icon: "mdi-account-tie" },
      ],
    };
  },
};
</script>

<style scoped>
sidebar {
  z-index: 10;
}
</style>
