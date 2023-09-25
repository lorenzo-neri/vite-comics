<script>
export default {
    name: "AppComicsSon",

    props: {
        lnThumb: String,
        lnPrice: String,
        lnSeries: String,
        lnType: String,
    },


    /* FUNZIONE PER IMPORTARE CORRETTAMENTE LE IMMAGINI DOPO UNA BUILD */
    methods: {
        getImageUrl(name) {
            return new URL(`${name}`, import.meta.url).href
        }
    } //#####

    /* ALLEGO SINTASSI BASE */
    /* function getImageUrl(name) {
    return new URL(`./dir/${name}.png`, import.meta.url).href
    } */
    /* https://vitejs.dev/guide/assets.html */
}
</script>

<template>
    <div class="card bg-transparent text-white border-0 p-1 py-2">
        <div class="square_image"> <!-- ##### -->
            <img :src="getImageUrl(lnThumb)" class="card-img-top" :alt="lnSeries">
        </div>
        <div class="card-body text-uppercase">
            <div>{{ lnSeries }}</div>
        </div>
    </div>
</template>
  
<style lang="scss" scoped>
.square_image {
    position: relative;
    width: 100%;
    padding-top: 100%;
    overflow: hidden;

    img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: auto;
    }
}

.card-body {
    font-size: .8rem;
}
</style>