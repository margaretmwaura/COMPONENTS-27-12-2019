<template>
    <div class="grid-frame" id="banner">

        <div class="grid-container">
            <div class="grid-x" id="banner_content">
                <div class="cell medium-1 large-1 small-1"></div>
                <div class="cell medium-6 large-5 small-10">
                    <p>{{message}}</p>
                    <br>
                    <buttonmine></buttonmine>
                </div>
                <div class="cell medium-1 large-6 small-1" ></div>
            </div>

        </div>
    </div>
</template>

<script>

    import buttonmine from './button'
    export default {
        name: "banner",
        components: {
            buttonmine
        },
        data() {
            return{
                message : "Empowering investors to discover & exploit the vast potential for wealth creation in Africa . "
            }
        }
    }
</script>

<style lang="scss">

    #banner {
        width: 100%;
        height: 560px;
        background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("../assets/banner.jpg");
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;

        &_content {

            p {
                color: white;
                font-size: 40px;
                margin-top: 150px;
                line-height: 1.1em;
            }


        }
    }
</style>
