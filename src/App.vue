<template>
  <v-app>
    <Navbar></Navbar>
    <Profil class="btn-profil"></Profil>
  </v-app>
</template>

<script>

import Profil from './components/Modifierprofil'
import Navbar from './components/Navbar'

export default {
  name: 'App',

  components: {
    Profil,
    Navbar
  },

  data: () => ({
    //
  }),
};
</script>

<style>
    .btn-profil{
      margin-top: 6.5%;
    }
</style>
