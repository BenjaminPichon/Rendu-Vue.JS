<template>
    <v-layout row wrap> 
        <v-flex lg4 v-for="image in images" :key='image.name'>
            <v-card flat height="400px">
                <img  class="imgsize" :src="image.src">
                <v-btn color="primary" @click="snackbar = true" class="btn-Save">Enregistrer</v-btn>
                <v-snackbar dark  v-model="snackbar" :timeout="timeout">
                    {{text}}
                    <v-btn color="red" text @click="snackbar = false">Close x</v-btn>
                </v-snackbar>
            </v-card>

        </v-flex>

    </v-layout>
</template>

<script>
export default {
    name : 'Actu',

    data() {
        return {
            snackbar: false,
            text: "Image Sauvegarder",
            timeout: 2000,
            images : [
                { name: '1',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg', desciption:'test'},
                { name: '2',src : 'https://www.mutualite.fr/content/uploads/2008/09/Nourriture-discount-comment-eviter-la-malbouffe-790x427.jpg'},
                { name: '3',src : 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg'},
                { name: '4',src : 'https://www.fourchette-et-bikini.fr/sites/default/files/styles/full_670x350/public/04fb8d17bc815f8c7105eef447e35998.jpg?itok=VBXvXnTf'},
                { name: '5',src : 'https://cdn.artphotolimited.com/images/59b65ee9faa2f46b71080369/300x300/manarola-by-night.jpg'},
                { name: '6',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { name: '7',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { name: '8',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { name: '9',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { name: '10',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { name: '11',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { name: '12',src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
            ]
        }
    }
}
</script>

<style>
    .imgsize {
        width: 95%;
    }
    .pos-card{
        margin-left: 50%;
    }
    .btn-Save{
        float: left;
    }
</style>