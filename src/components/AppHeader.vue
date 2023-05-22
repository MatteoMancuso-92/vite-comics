<script>
import AppNav from './AppNav.vue';
export default {
  
  components: {
    AppNav,
  }
}
</script>

<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="">
    <AppNav />
  </header>
</template>

<style lang="scss" scoped>
@use './../assets/styles/partials/variables' as *;

header{
  width: 70%;
  height: 130px;
  @include align-justify-center;
  img{
    height: 90px;
  } 
}
</style>