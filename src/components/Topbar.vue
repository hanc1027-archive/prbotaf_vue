<template>
  <v-app-bar color="red lighten-3" dark fixed app>
    <router-link to="/" style="text-decoration: none; color: inherit">
      <v-toolbar-title>青年班《耳根圓通》登錄簿</v-toolbar-title></router-link
    >
    <v-spacer></v-spacer>
    <div class="d-none d-md-block">
      <router-link to="/" style="text-decoration: none; color: inherit">
        <v-btn class="ma-2" outlined color="indigo">
          部數登錄
        </v-btn></router-link
      >
      <router-link to="/query" style="text-decoration: none; color: inherit">
        <v-btn class="ma-2" outlined color="indigo">
          部數查詢
        </v-btn></router-link
      >
      <v-btn
        class="ma-2"
        outlined
        color="indigo"
        :href="second_link"
        target="_blank"
      >
        楞嚴咒
      </v-btn>
      <v-btn
        class="ma-2"
        outlined
        color="indigo"
        :href="third_link"
        target="_blank"
      >
        耳根圓通
      </v-btn>
    </div>

    <div class="d-md-none">
      <v-menu offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-app-bar-nav-icon v-bind="attrs" v-on="on"> </v-app-bar-nav-icon>
        </template>
        <v-list style="float: right" class="d-md-none">
          <v-list-item>
            <router-link to="/" style="text-decoration: none; color: inherit">
              <v-btn class="ma-2" outlined color="indigo">
                部數登錄
              </v-btn></router-link
            ></v-list-item
          >
          <v-list-item
            ><router-link
              to="/query"
              style="text-decoration: none; color: inherit"
            >
              <v-btn class="ma-2" outlined color="indigo">
                部數查詢
              </v-btn></router-link
            ></v-list-item
          >
          <v-list-item
            ><v-btn
              class="ma-2"
              outlined
              color="indigo"
              :href="second_link"
              target="_blank"
            >
              楞嚴咒
            </v-btn></v-list-item
          >
          <v-list-item
            ><v-btn
              class="ma-2"
              outlined
              color="indigo"
              :href="third_link"
              target="_blank"
            >
              耳根圓通
            </v-btn></v-list-item
          >
        </v-list>
      </v-menu>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      isHome: true,
      second_link:
        "https://drive.google.com/file/d/15Zx_LBGW2lToj2C7Nlz5qW3wZ-EEajwC/view?usp=sharing", //楞嚴咒
      third_link:
        "https://drive.google.com/file/d/1CalP3rk80yNdO7Dl862w0mHEK6SpsnMx/view?usp=sharing", //耳根圓通
    };
  },
};
</script>

<style>
</style>