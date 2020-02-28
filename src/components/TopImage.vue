<template>
    <div class="carousel">
        <v-carousel cycle interval="3000" hide-delimiter-background show-arrows-on-hover delimiter-icon="mdi-minus">
            <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src"></v-carousel-item>
        </v-carousel>
    </div>
    
</template>

<script>
export default {
    name: 'Carousel',

    data(){
        return {
            items : [
                { src : 'https://cdn.pixabay.com/photo/2017/12/26/07/36/nature-3039901_960_720.jpg'},
                { src : 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg'},
                { src : 'https://cdn.artphotolimited.com/images/59b65ee9faa2f46b71080369/300x300/manarola-by-night.jpg'},
                { src : 'https://www.fourchette-et-bikini.fr/sites/default/files/styles/full_670x350/public/04fb8d17bc815f8c7105eef447e35998.jpg?itok=VBXvXnTf'},
                { src : 'https://www.mutualite.fr/content/uploads/2008/09/Nourriture-discount-comment-eviter-la-malbouffe-790x427.jpg'},

            ]
        }
    }
}
</script>

<style>
    .carousel{
        width: 75%;
        
        
    }
</style>