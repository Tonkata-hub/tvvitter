<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer">
      <v-btn
        elevation="2"
        class="btn"
        size="large"
      ><router-link to="/">Home</router-link></v-btn>
      <v-btn
        elevation="2"
        class="btn"
        size="large"
      ><router-link to="/register">Register</router-link></v-btn>
      <v-btn
        elevation="2"
        class="btn"
        size="large"
      ><router-link to="/">Profile</router-link></v-btn>
      <v-btn
        elevation="2"
        class="btn"
        size="large"
      ><router-link to="/">Settings</router-link></v-btn>
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