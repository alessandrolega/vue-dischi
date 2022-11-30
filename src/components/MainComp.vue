<template>
    <main class="container">
        <!--COMPONENT ALBUM LIST-->
        <AlbumsList/>
    </main>
</template>

<script>

import AlbumsList from './albums/AlbumsList.vue'

    export default {
        name: 'MainComp',
        components: {
            AlbumsList
        }
    }
</script>

<style lang="scss" scoped>

main{
    height: 95%;
    background-color: #1e2d3b;
    color: white;
}

</style>