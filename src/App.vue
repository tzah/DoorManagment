<template>
  <v-app>
    <login-page />
  </v-app>
</template>

<script>
import LoginPage from "./components/LoginPage/loginPage.vue";

export default {
  name: "App",

  components: {
    LoginPage,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
.border {
  border: red 2px solid;
}
</style>
