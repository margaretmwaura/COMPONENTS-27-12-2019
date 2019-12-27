<template>
    <div class="grid-frame">
    <div class="grid-container" id="top">
        <div id="top_nav_bar">
            <div id="responsive-menu">
                <div id="top_nav_bar_navbar" class="grid-container">
                    <div class="menu dropdown align-center grid-x" data-dropdown-menu>
                        <div class="cell large-1"></div>
                        <div class="cell medium-6 small-12 large-10" id="top_nav_bar_navbar_links">
                            <img src="../assets/logo.png">
                            <ul class="menu dropdown align-center" data-dropdown-menu>
                                <li v-for="nav in navigations" :key="nav.id">
                                    <a href="#">{{nav.name}}</a>
                                </li>
                                <li><a href="#"><i class="fi-magnifying-glass"></i> <span></span></a></li>
                            </ul>
                        </div>
                        <div class="cell large-1"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
    export default {
        name: "navigation",
        props:['navigations']
    }
</script>

<style lang="scss">
    #top {

        &_nav_bar {

            &_navbar {

                &_links {
                    img {
                        height: 75px;
                        width: 75px;
                        float: left;
                    }

                    ul {
                        padding-top: 15px;
                        float: right;

                        li {
                            padding-left: 0px;
                            padding-right: 0px;
                            margin-left: 0px;
                            margin-right: 0px;

                            a {
                                color: #5C213C;
                                font-size: 15px;
                            }

                            a:hover {
                                border-bottom: 5px solid #000000;
                            }

                        }
                    }

                }

            }
        }
    }
</style>
