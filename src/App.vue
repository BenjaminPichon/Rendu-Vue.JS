<template>
  <v-app>
    <Navbar></Navbar>
    <Profil class="btn-profil"></Profil>
    <hr class="separation" width="50%">
    <Carousel class="pos-carousel"></Carousel>
    <hr class="separation" width="50%">
  </v-app>
</template>

<script>

import Profil from './components/Modifierprofil'
import Navbar from './components/Navbar'
import Carousel from './components/TopImage'

export default {
  name: 'App',

  components: {
    Profil,
    Navbar,
    Carousel
  },

  data: () => ({
    //
  }),
};
</script>

<style>
    .btn-profil{
      margin-top: 6.5%;
      margin-right: 0%;
    }
    .pos-carousel{
      margin-left: 12.5%;
    }
    .separation{
      margin-top: 10%;
      margin-bottom: 10%;
      margin-left: 25%
      
    }
</style>
