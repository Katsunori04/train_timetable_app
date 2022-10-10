<template>
  <v-app>
      <!-- ヘッダー -->
      <header>
        <v-app-bar color="blue-grey darken-4"  height="80">
          <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
          <v-toolbar-title class="red--text">LOGO</v-toolbar-title>
        </v-app-bar>
        <v-navigation-drawer v-model="drawer" fixed temporary>
          <v-list nav dense>
            <v-list-item-group>
              <v-list-item link to="/">
                <v-list-item-title>HOME</v-list-item-title>
              </v-list-item>
              <v-list-item>
                <v-list-item-title>ABOUT</v-list-item-title>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-navigation-drawer>
      </header>

    <v-main>
      <router-view />
    </v-main>

    <!-- フッター -->
    <v-footer color="blue-grey darken-4" dark app height="50" absolute>テストサイト</v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    drawer: false,
    //
  }),
};
</script>
