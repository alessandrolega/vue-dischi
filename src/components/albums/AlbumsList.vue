<template>
    <div id="Albumslist" class="d-flex flex-direction-row justify-content-between align-items-center mt-4 row-cols-5">
        <AlbumCard v-for="(element, index) in albums"
         :key="index"
         :cardProp="element"/>
        
    </div>
</template>

<script>

import AlbumCard from './AlbumCard.vue'
import axios from 'axios'

    export default {
        name: 'AlbumsList',
        components: {
            AlbumCard
        },
        data(){
            return {
                albums: []

        }
        },
        mounted(){
            axios.get('https://flynn.boolean.careers/exercises/api/array/music')
            .then((response)=>{
                this.albums = response.data.response
            })
    
    }
    }
</script>

<style lang="scss" scoped>

#Albumslist{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}


</style>