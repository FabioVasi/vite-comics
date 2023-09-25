<script>
  import LogoComics from './LogoComics.vue';
  export default {
    data() {
      return {
        name: 'Header'
      }
    },
    components: {
      LogoComics
    }
  }
</script>

<template>

  <header id="header_comics" class="d-flex align-items-center">

    <div class="container h-100 p-0 d-flex justify-content-between align-items-center">
      <LogoComics/>
      <nav class="navbar p-0 h-100 navbar-expand">
          <ul class="nav navbar-nav">
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">CHARACTERS</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5 active" href="#" aria-current="page">COMICS</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">MOVIES</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">TV</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">GAMES</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">COLLECTIBLES</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">VIDEOS</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">FANS</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">NEWS</a>
            </li>
            <li class="nav-item fw-bold fs-5">
              <a class="nav-link pt-5 pb-5" href="#">SHOP</a>
            </li>
          </ul>
      </nav>
    </div>

  </header>

</template>

<style lang="scss" scoped>

  @use '../assets/scss/partials/variable.scss' as *;

  #header_comics{
    height: 150px;

    a.active {
      color: $color_dclogo;
      border-color: $color_dclogo;
      border-bottom: 0.5rem solid;
      
    }
    .nav-link:hover{
        color: $color_dclogo;
        border-color: $color_dclogo;
        border-bottom: 0.5rem solid;
    }
    .nav-link{

    }
  }

</style>
