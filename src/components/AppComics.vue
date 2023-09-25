<script>
import comics from '../comics.js';

export default {

    name: 'AppComics',

    data() {
        return {
            comics: comics
        }
    }
}
</script>

<template>
    <!-- TODO modifica sintassi immagini per build -->
    <div class="col-md-2" v-for="comic in comics">

        <div class="card">
            <img :src="comic.thumb" class="card-img-top" :alt="comic.series">
            <div class="card-body">
                <div>{{ comic.series }}</div>
            </div>
        </div>

    </div>
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/app.scss' as *;
</style>