<script>
  export default {
    data() {
      return {
        card: '',
        cards: [
            {
                name: 'DIGITAL COMICS',
                image: 'src/assets/img/buy-comics-digital-comics.png'
            },
            {
                name: 'DC MERCHANDISE',
                image: 'src/assets/img/buy-comics-merchandise.png'
            },
            {
                name: 'SUBSCRIPTION',
                image: 'src/assets/img/buy-comics-subscriptions.png'
            },
            {
                name: 'COMIC SHOP LOCATOR',
                image: 'src/assets/img/buy-comics-shop-locator.png'
            },
            {
                name: 'DC POWER VISA',
                image: 'src/assets/img/buy-dc-power-visa.svg'
            },
            
        ]
      }
    }
  }
</script>

<template>

    <main id="main_comics">

        <div class="container p-0">
            <h1 class="text-white pt-5 pb-5 m-0">Content goes here</h1>
        </div>

        <div class="merchandise position-relative">
            <div class="container ps-0 pe-0 pt-5 pb-5 d-flex justify-content-between align-items-center">

                <a v-for="card in cards" class="text-white text-decoration-none" href="#">
                    <img style="height: 80px;" :src="card.image" alt="">
                    <span class="ps-3">{{card.name}}</span>
                </a>
        
            </div>
        </div>

        <div class="heroes d-flex">
            <div class="container p-0 d-flex justify-content-between">
                <div class="d-flex justify-content-evenly">
                    <ul class="lists list-unstyled pt-4 m-0 pb-5 pe-5">
                    <li>
                        <h3 class="text-white pt-3 pb-3 m-0">DC COMICS</h3>
                    </li>
                    <li class="fw-medium pt-1 pb-1">Characters</li>
                    <li class="fw-medium pt-1 pb-1">Comics</li>
                    <li class="fw-medium pt-1 pb-1">Movies</li>
                    <li class="fw-medium pt-1 pb-1">TV</li>
                    <li class="fw-medium pt-1 pb-1">Games</li>
                    <li class="fw-medium pt-1 pb-1">Videos</li>
                    <li class="fw-medium pt-1 pb-1">News</li>
                    <li>
                        <h3 class="text-white pt-3 pb-3 m-0">SHOP</h3>
                    </li>
                    <li class="fw-medium pt-1 pb-1">Shop DC</li>
                    <li class="fw-medium pt-1 pb-1">Shop DC Collectibles</li>
                    </ul>
                    <ul class="lists list-unstyled pt-4 m-0 pb-5 pe-5">
                        <li>
                            <h3 class="text-white pt-3 pb-3 m-0">DC</h3>
                        </li>
                        <li class="fw-medium pt-1 pb-1">Terms Of Use</li>
                        <li class="fw-medium pt-1 pb-1">Privacy policy (New)</li>
                        <li class="fw-medium pt-1 pb-1">Ad Choices</li>
                        <li class="fw-medium pt-1 pb-1">Advertising</li>
                        <li class="fw-medium pt-1 pb-1">Jobs</li>
                        <li class="fw-medium pt-1 pb-1">Subscriptions</li>
                        <li class="fw-medium pt-1 pb-1">Talent Workshops</li>
                        <li class="fw-medium pt-1 pb-1">CPSC Certificates</li>
                        <li class="fw-medium pt-1 pb-1">Ratings</li>
                        <li class="fw-medium pt-1 pb-1">Shop Help</li>
                        <li class="fw-medium pt-1 pb-1">Contact Us</li>
                    </ul>
                    <ul class="lists list-unstyled pt-4 m-0 pb-5 pe-5">
                        <li>
                            <h3 class="text-white pt-3 pb-3 m-0">SITES</h3>
                        </li>
                        <li class="fw-medium pt-1 pb-1">DC</li>
                        <li class="fw-medium pt-1 pb-1">MAD Magazine</li>
                        <li class="fw-medium pt-1 pb-1">DC Kids</li>
                        <li class="fw-medium pt-1 pb-1">DC Universe</li>
                        <li class="fw-medium pt-1 pb-1">DC Power Visa</li>
                    </ul>
                </div>            
                <img class="dc-logo-bg" src="../assets/img/dc-logo-bg.png" alt="">
            </div>        
        </div>

    </main>

</template>

<style lang="scss">


</style>