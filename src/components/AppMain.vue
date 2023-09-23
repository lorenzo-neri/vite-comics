<script>
export default {

    name: 'AppMain',

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
    <div id="jumbotron">
        <div class="container">
            <h2>Content goes here</h2>
        </div>
    </div>
    <!-- /#jumbotron -->

    <div id="sections_bar">
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
    </div>
    <!-- /#sections_bar -->
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/app.scss' as *;

* {
    color: $dc-white;
}

#jumbotron {
    background-color: $dc-black;
    padding: 3rem 0;
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