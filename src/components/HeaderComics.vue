<script>
  import LogoComics from './LogoComics.vue';
  export default {
    data() {
      return {
        
      }
    },
    components: {
      LogoComics
    }
  }
</script>

<template>

  <header id="header_comics" class="d-flex align-items-center">

    <div class="container p-0 d-flex justify-content-between align-items-center">
      <LogoComics/>
      <nav class="navbar navbar-expand">
          <ul class="nav navbar-nav">
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">CHARACFTERS</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link active" href="#" aria-current="page">COMICS<span class="visually-hidden">(current)</span></a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">MOVIES</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">TV</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">GAMES</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">COLLECTIBLES</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">VIDEOS</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">FANS</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">NEWS</a>
            </li>
            <li class="nav-item fw-bold fs-4">
              <a class="nav-link" href="#">SHOP</a>
            </li>
          </ul>
      </nav>
    </div>

  </header>

</template>

<style lang="scss">

  @use '../assets/scss/partials/variable.scss' as *;

  #header_comics{
    height: 150px;

    a.active {
      color: $color_dclogo;
      border-color: $color_dclogo;
      border-bottom: 0.5rem solid;
    }
  }

</style>
