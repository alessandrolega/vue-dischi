<template>
  <div id="app">
    <!--HEADER-->
    <HeaderComp/>
    <!--MAIN-->
    <MainComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp
  },
}
</script>

<style lang="scss">
#app{
  height: 100vh;
  background-color: #1e2d3b;
}

</style>
