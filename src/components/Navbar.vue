<template>
  <div>
    <v-app-bar
      absolute
      color="blue darken-3"
      dark
      prominent
    >
      <v-toolbar-title></v-toolbar-title>

      <v-spacer></v-spacer>

      <div class="profil">
        <v-badge
          color="red"
          content="9+"
        >
          <v-avatar color="light-green" size="42">
            
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
