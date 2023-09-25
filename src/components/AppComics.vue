<script>
import comics from '../comics.js';
import AppComicsSon from './AppComicsSon.vue';

export default {

    name: 'AppComics',

    components: { AppComicsSon },

    data() {
        return {
            comics,
        }
    }
}
</script>

<template>
    <!-- TODO modifica sintassi immagini per build -->
    <div class="col-2 pt-2" v-for="comic in comics">

        <AppComicsSon :lnThumb="comic.thumb" :lnPrice="comic.price" :lnSeries="comic.series" :lnType="comic.type" />

        <!-- IL MARKUP VA NEL COMPONENTE FIGLIO -->
        <!-- <div class="card">
            <img :src="comic.thumb" class="card-img-top" :alt="comic.series">
            <div class="card-body">
                <div>{{ comic.series }}</div>
            </div>
        </div> -->

    </div>
</template>

<style lang="scss" scoped></style>