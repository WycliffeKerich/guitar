<template>
  <v-toolbar>
    <v-app-bar-nav-icon to="home"></v-app-bar-nav-icon>

    <v-toolbar-title><v-btn color="primary" to="home">TabTracker</v-btn></v-toolbar-title>

    <v-spacer></v-spacer>
    <v-spacer></v-spacer>
    <v-spacer></v-spacer>
    <v-spacer></v-spacer>

    <v-btn
      v-if="!$store.state.isUserLoggedIn"
      to="register"
      color="primary" >
      Register
    </v-btn>

    <v-spacer></v-spacer>

    <v-btn
      v-if="!$store.state.isUserLoggedIn"
      to="login"
      color="primary" >
      Login
    </v-btn>

    <v-spacer></v-spacer>

    <v-btn icon>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>
  </v-toolbar>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped>

</style>
