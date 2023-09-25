<script>

  import HeaderComics from "./components/HeaderComics.vue";
  import LogoComics from "./components/LogoComics.vue";
  import MainComics from "./components/MainComics.vue";
  import FooterComics from "./components/FooterComics.vue";
  import ComicItem from "./components/ComicItem.vue";
  
  export default {
    components: {
      HeaderComics,
      LogoComics,
      MainComics,
      ComicItem,
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
