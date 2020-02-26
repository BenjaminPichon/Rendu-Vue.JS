<template>
    <div class="carousel">
        <v-carousel hide-delimiter-background show-arrows-on-hover delimiter-icon="mdi-minus">
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
                { src : 'https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.lanouvellerepublique.fr%2Fa-la-une%2Fle-paysage-une-therapie&psig=AOvVaw3WbrFYACs1buI0YmM7IdUd&ust=1582819962698000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNi1joDO7-cCFQAAAAAdAAAAABAD'},
                { src : 'https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.lanouvellerepublique.fr%2Fa-la-une%2Fle-paysage-une-therapie&psig=AOvVaw3WbrFYACs1buI0YmM7IdUd&ust=1582819962698000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNi1joDO7-cCFQAAAAAdAAAAABAD'},
                { src : 'https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.lanouvellerepublique.fr%2Fa-la-une%2Fle-paysage-une-therapie&psig=AOvVaw3WbrFYACs1buI0YmM7IdUd&ust=1582819962698000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNi1joDO7-cCFQAAAAAdAAAAABAD'},
                { src : 'https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.lanouvellerepublique.fr%2Fa-la-une%2Fle-paysage-une-therapie&psig=AOvVaw3WbrFYACs1buI0YmM7IdUd&ust=1582819962698000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNi1joDO7-cCFQAAAAAdAAAAABAD'},

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