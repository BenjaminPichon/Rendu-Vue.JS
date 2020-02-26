<template>
  <div>
    <v-app-bar
      absolute
      color="deep-purple accent-4"
      dark
      prominent
      shrink-on-scroll=""
    >
      <v-toolbar-title></v-toolbar-title>

      <v-spacer></v-spacer>

      <div class="profil">
        <v-badge
          color="green"
          content="6"
        >
          <v-avatar color="blue" size="42">
            
            <v-icon dark>mdi-account-circle</v-icon>
            
          </v-avatar>
        </v-badge>
      </div>
      
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name : 'Navbar',
}
</script>

<style>
    .profil{
      margin: 2%;
    }
</style>
