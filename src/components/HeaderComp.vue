<template>
  <header>
    <img src="../assets/logo-small.svg" alt="">
  </header>
</template>

<script>
export default {
  name: 'HeaderComp',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

header{
  background-color: #2e3a46;
  color: white;
  height: 5%;
}

header > img{
  width: 30px;
  margin: 10px;
}

</style>
