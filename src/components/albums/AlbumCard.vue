<template>
    <div class="">
        <div class="card">
            <img :src="cardProp.poster" class="card-img-top" alt="card-img">
            <div class="card-body">
                <div class="text-center">
                    <h5 class="card-title">{{cardProp.title}}</h5>
                    <span>{{cardProp.author}}</span>
                    <span>{{cardProp.year}}</span>
                </div>
            </div>
        </div>
    </div>
    
</template>

<script>
    export default {
        name: 'AlbumCard',
        props: {
            cardProp : Object
        }
    }
</script>

<style lang="scss" scoped>

.card{
    background-color: #2e3a46;
    width: 80%;
  
}

</style>