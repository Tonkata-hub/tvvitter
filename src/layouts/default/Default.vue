<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer">
      <v-btn
        v-for="nav in navButtons"
        elevation="2"
        class="btn"
        size="large"
      >{{ nav }}</v-btn>
    </v-navigation-drawer>

    <v-app-bar>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Tvvitter</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data (){ 
      return {
        drawer: null,
        navButtons: [
          'Home',
          'Profile',
          'Settings'
        ],
      }
    }
  }
</script>

<style scoped>
  .btn {
    display: block;
    margin: 15px auto;
    width: 150px;
  }
</style>