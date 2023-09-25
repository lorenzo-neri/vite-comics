<script>
import AppComics from './AppComics.vue';

export default {

    name: 'AppMain',

    components: {
        AppComics
    },

    data() {
        return {
            cardsArray: [
                { title: 'DIGITALS COMICS', image: '../../src/assets/img/buy-comics-digital-comics.png' },
                { title: 'DC MERCHANDISE', image: '../../src/assets/img/buy-comics-merchandise.png' },
                { title: 'SUBCRIPTION', image: '../../src/assets/img/buy-comics-subscriptions.png' },
                { title: 'COMIC SHOP LOCATOR', image: '../../src/assets/img/buy-comics-shop-locator.png' },
                { title: 'DC POWER VISA', image: '../../src/assets/img/buy-dc-power-visa.svg' }
            ]
        }
    }
}
</script>

<template>
    <!-- TODO modifica sintassi immagini per build -->
    <section id="jumbotron">

    </section>
    <!-- /#jumbotron -->


    <section id="app_comics">

        <div class="container">

            <span class="section_comics blue_ticket">
                CURRENT SERIES
            </span>

            <div class="row px-2 py-3 justify-content-center">



                <AppComics />



            </div>

            <div class="d-flex justify-content-center">
                <span class="blue_ticket text-center mb-3">
                    <a class="text-decoration-none text-white" href="##">LOAD MORE</a>
                </span>
            </div>
        </div>
    </section>
    <!-- /#app_comics -->

    <section id="sections_bar">
        <div class="container">
            <div class="row p-5">

                <div class="col d-flex justify-content-center align-items-center gap-2 p-3"
                    v-for="(card, i) in this.cardsArray">
                    <img :src="card.image" alt="" class="">
                    <div id="title" class="fw-semibold">{{ card.title }}</div>
                </div>

            </div>
            <!-- /.row -->
        </div>
        <!-- /.container -->
    </section>
    <!-- /#sections_bar -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/app.scss' as *;

* {
    color: $dc-white;
}

#jumbotron {

    background-image: url(../../src/assets/img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
    height: 500px;
}

#app_comics {
    background-color: $dc-black;
    position: relative;

    .section_comics {
        position: absolute;
        top: -30px;

    }
}

.blue_ticket {
    color: white;
    background-color: $dc-primary;
    padding: .5rem 1.5rem;
    font-weight: 800;
    scale: 1.1;
}

#sections_bar {
    background-color: $dc-primary;

    img {
        width: 3rem;
    }

    #title {
        font-size: .8rem;
    }
}
</style>