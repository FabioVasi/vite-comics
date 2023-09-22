<script>
  export default {
    data() {
      return {
        
      }
    }
  }
</script>

<template>

    <footer id="footer_comics" class="d-flex align-items-center">
        <div class="container p-0 d-flex justify-content-between align-items-center">
            <a href="#">
                <button class="text-white">SIGN-UP NOW!</button>
            </a>
            <div class="d-flex justify-content-between align-items-center">
                <a class="pe-3 text-decoration-none" href=""><h3>FOLLOW US</h3></a>
                <a class="pe-3" href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                <a class="pe-3" href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                <a class="pe-3" href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                <a class="pe-3" href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                <a class="pe-3" href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
            </div>
            
        </div>

    </footer>

</template>

<style lang="scss">

    @use '../assets/scss/partials/variable.scss' as *;

    #footer_comics{
        background-color: $bg_dcfooter;
        height: 150px;
        margin-top: -100px;
        position: relative;
        a button{
            background-color: $bg_dcfooter;
            text-decoration: none;
            border: 3px solid $color_dclogo;
            font-size: 20px;
            padding: 1rem 1.50rem;
        }
    }

</style>