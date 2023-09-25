<script>
import comics from "../comics.js"; // array of comics import
import ComicItem from "./ComicItem.vue"; // import comics components connection 
  export default {
    name: 'MainComics',
    components: {
        ComicItem
    },
    data() {
      return {
        comics,
        card: '', //merchandise
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
            
        ],
        list: '', //first list
        lists: [
            {
                link: 'Characters'
            },
            {
                link: 'Comics'
            },
            {
                link: 'Movies'
            },
            {
                link: 'TV'
            },
            {
                link: 'Games'
            },
            {
                link: 'Videos'
            },
            {
                link: 'News'
            }            
        ],
        info: '', // second list
        information: [
            {
                about: 'Terms Of Use'
            },
            {
                about: 'Privacy policy (New)'
            },
            {
                about: 'Ad Choices'
            },
            {
                about: 'Advertising'
            },
            {
                about: 'Jobs'
            },
            {
                about: 'Subscriptions'
            },
            {
                about: 'Talent Workshops'
            },
            {
                about: 'CPSC Certificates'
            },
            {
                about: 'Ratings'
            },
            {
                about: 'Shop Help'
            },
            {
                about: 'Contact Us'
            }
        ],
        site: '', // third list
        sites: [
            {
                source: 'DC'
            },
            {
                source: 'MAD Magazine'
            },
            {
                source: 'DC Kids'
            },
            {
                source: 'DC Universe'
            },
            {
                source: 'DC Power Visa'
            }
        ]
      }
    },
    created() {
        console.log(this.comics);
    }
  }
</script>

<template>

    <main id="main_comics">

        <div class="jumbotron"></div>

        <div class="container p-0 text-center pb-3">
            <div class="row row-cols-1 row-cols-sm-3 row-cols-md-6">

                <ComicItem v-for="comic in comics" :image="comic.thumb" :title="comic.title" :price="comic.price" :type="comic.type"/>
                
            </div>           
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
                        <li v-for="list in lists" class="fw-medium pt-1 pb-1">{{list.link}}</li>
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
                        <li v-for="info in information" class="fw-medium pt-1 pb-1">{{info.about}}</li>
                    </ul>

                    <ul class="lists list-unstyled pt-4 m-0 pb-5 pe-5">
                        <li>
                            <h3 class="text-white pt-3 pb-3 m-0">SITES</h3>
                        </li>
                        <li v-for="site in sites" class="fw-medium pt-1 pb-1">{{site.source}}</li>
                    </ul>
                </div>            
                <img class="dc-logo-bg" src="../assets/img/dc-logo-bg.png" alt="">
            </div>        
        </div>

    </main>

</template>

<style lang="scss" >


</style>