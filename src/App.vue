<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {

    name: 'App',
    data() {
        return {

        }
    },
    components: {

        AppHeader,
        AppMain,
    }

}
</script>

<template>
    <header>
        <div class="container">
            <AppHeader></AppHeader>
        </div>
    </header>
    <AppMain></AppMain>
</template>

<style lang="scss" scoped>
@import '../src/assets/scss/app.scss';

/* ho trovato un altro metodo per suddividere l'header e dargli un colore di sfondo ma è più scomdo */
header {
    background-color: $dc-white;
}
</style>
