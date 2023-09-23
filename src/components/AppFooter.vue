<script>
export default {

    name: 'AppFooter',

    data() {
        return {
            footerSections: [
                { titleSection: 'DC COMICS', info: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'] }
            ]
        }
    }
}
</script>

<template>
    <div id="footer_top">
        <div class="container">
            <div class="row">
                <div class="col-6 text-white">
                    <div class="col-9 d-flex flex-wrap flex-column">
                        <div class="col-3">
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. A molestiae repellat incidunt beatae
                            quidem pariatur impedit odio minima numquam consectetur, similique at voluptatum ipsa iure quos
                            placeat, veniam optio animi.
                        </div>


                    </div>
                    <!-- /.col-9 -->
                </div>
                <!-- /.col-6 -->
                <div class="col-6 d-flex justify-content-end">
                    <div id="bg_logo" class="col-10 ">

                    </div>
                </div>
                <!-- /.col-6 -->
            </div>
            <!-- /.row -->

        </div>

    </div>
    <!-- /#footer_top -->
    <div id="footer_bottom"></div>
    <!-- /#footer_bottom -->
</template>

<style lang="scss" scoped>
#footer_top {
    background-image: url(../../src/assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;

    .row {
        height: 400px;
    }

    #bg_logo {
        background-image: url(../../src/assets/img/dc-logo-bg.png);
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }
}
</style>