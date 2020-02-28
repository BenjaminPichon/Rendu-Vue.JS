<template>
  <v-app>
    <Navbar></Navbar>
    <Profil class="btn-profil"></Profil>
    <hr class="separation" width="50%">
    <h2 class="partieTitle">Top de la semaine</h2>
    <Carousel class="pos-carousel"></Carousel>
    <hr class="separation" width="50%">
    <h2 class="partieTitle">Fil d'actualité</h2>
    <Actu class="posActu"></Actu>
  </v-app>
</template>

<script>

import Profil from './components/Modifierprofil'
import Navbar from './components/Navbar'
import Carousel from './components/TopImage'
import Actu from './components/filActus'

export default {
  name: 'App',

  components: {
    Profil,
    Navbar,
    Carousel,
    Actu
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
    .partieTitle {
      text-align: center;
      margin-bottom: 5%;
      font-size: 200%;
      color: darkred;
    }
    .posActu{
      text-align: center;
      width: 75%;  
      margin-left: 12.5%; 
    }
</style>
