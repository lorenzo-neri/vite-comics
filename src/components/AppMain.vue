<script>
export default {

    name: 'AppMain',

    data() {
        return {
            cardsArray: [
                { title: 'DIGITALS COMICS', image: '../../src/assets/img/buy-comics-digital-comics.png' },
                { title: 'DC MERCHANDISE', image: '../../src/assets/img/buy-comics-merchandise.png' },
                { title: 'SUBCRIPTION', image: '' }
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
            <div></div>
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
}
</style>