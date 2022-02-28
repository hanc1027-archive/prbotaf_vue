<template>
  <v-app>
    <TopBar />
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import TopBar from "./components/Topbar.vue";
export default {
  name: "App",
  components: {
    TopBar,
  },
};
</script>

<style scoped>
#app {
  /* font-size: 1.3em; */
  font-family: Work Sans;
}
</style>
