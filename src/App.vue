<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';


export default {

    name: 'App',
    data() {
        return {

        }
    },
    components: {
        Header,
        Main,
    }

}
</script>

<template>
    <div class="container">
        <Header></Header>
        <Main></Main>
    </div>
</template>

<style lang="scss"></style>
