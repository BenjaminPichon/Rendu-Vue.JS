<template>
  <v-row justify="end">
    <v-dialog v-model="dialog" persistent max-width="600px" transition="scroll-x-transition">
      <template v-slot:activator="{ on }">
        <v-btn color="blue darken-2" dark v-on="on">Modifier les informations du Profil</v-btn>
      </template>
      <v-card>
        <v-card-title>
          <span class="headline">Information du profil</span>
        </v-card-title>
        <v-card-text>
          <v-container>
            <v-row>
              <v-col cols="12" sm="6" md="4">
                <v-text-field label="Prenom" required></v-text-field>
              </v-col>
             
              <v-col cols="12" sm="6" md="4">
                <v-text-field
                  label="Nom"
                  required
                ></v-text-field>
              </v-col>
              <v-col cols="12" sm="6" md="4">
                <input @click="hidden=true" type="checkbox" id="privated" value="privated" v-model="hidden"> 
                <label for="privated">Je veux masquer mes Interet</label>
              </v-col>
              <v-col cols="12">
                <v-text-field label="Email" required></v-text-field>
              </v-col>
              <v-col cols="12">
                <v-text-field label="Mot de passe" type="password" required></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-select 
                  :items="['0-17', '18-29', '30-54', '54+']"
                  label="Age"
                  required
                ></v-select>
              </v-col>
              <v-col cols="12" sm="6">
                <v-autocomplete 
                  :items="['Manga', 'Tattoo', 'Dessin', 'Art', 'Nourriture', 'Photo']"
                  v-if="hidden===false"
                  label="Interet"
                  multiple
                ></v-autocomplete>
                <h4 class="privé" v-else>C'est privé</h4>
              </v-col>
            </v-row>
          </v-container>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="blue darken-1" text @click="dialog = false">Close</v-btn>
          <v-btn color="blue darken-1" text @click="dialog = false">Save</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
  export default {
    name : 'Profil',
    
    data: () => ({
      dialog: false,
      hidden: false,
    }),
  }
</script>

<style>
    .privé{
      margin-top: 11%;
      margin-left: 25%;
    }
</style>