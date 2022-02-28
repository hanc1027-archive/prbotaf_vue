<template>
  <v-app>
    <v-app-bar color="red lighten-3" dark fixed app>
      <v-toolbar-title>青年班《耳根圓通》登錄簿</v-toolbar-title>
      <v-spacer></v-spacer>
      <div class="d-none d-md-block">
        <v-btn class="ma-2" outlined color="indigo"> 部數查詢 </v-btn>
        <v-btn class="ma-2" outlined color="indigo"> 楞嚴咒 </v-btn>
        <v-btn class="ma-2" outlined color="indigo"> 耳根圓通 </v-btn>
      </div>

      <div class="d-md-none">
      <v-menu offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-app-bar-nav-icon v-bind="attrs" v-on="on"></v-app-bar-nav-icon>
        </template>
        <v-list>
           <v-btn class="ma-2" outlined color="indigo"> 部數查詢1 </v-btn>
        <v-btn class="ma-2" outlined color="indigo"> 楞嚴咒 </v-btn>
        <v-btn class="ma-2" outlined color="indigo"> 耳根圓通 </v-btn>
        </v-list>
      </v-menu>
     </div>
    </v-app-bar>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      menu: [
        { icon: "home", title: "Link A" },
        { icon: "info", title: "Link B" },
        { icon: "warning", title: "Link C" },
      ],
    };
  },
};
</script>

<style scoped>
#app {
  /* font-size: 1.3em; */
  font-family: Work Sans;
}
</style>
