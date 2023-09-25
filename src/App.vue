<script>

  import HeaderComics from "./components/HeaderComics.vue";
  import LogoComics from "./components/LogoComics.vue";
  import MainComics from "./components/MainComics.vue";
  import FooterComics from "./components/FooterComics.vue";
  import Comic from "./components/Comic.vue";
  
  export default {
    components: {
      HeaderComics,
      LogoComics,
      MainComics,
      Comic,
      FooterComics
    }
  }

</script>

<template>

  <HeaderComics/>
  <MainComics/>
  <FooterComics/>

</template>

<style lang="scss">

</style>
