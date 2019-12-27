<template>
    <div class="grid-container">
        <div class="grid-x grid-margin-x" id="content">
            <div class="cell small-0 large-1 medium-1"></div>
            <div class="cell small-6 large-5 medium-5" id="content_one">
                <p id="one"> Stock Brokerage</p>

                <p id="two">AIB has appointed security representatives and investors Agents countrywide to extend its reach.
                    Such agents and representatives have undergone appropriate training on how to approch and assist propspecive
                    investors</p>

                <button>
                    Find Out More <span> <i class="fa fa-angle-right"></i></span>
                </button>
            </div>
            <div class="cell small-6 large-5 medium-5" id="content_two">
                <p> Mobile and Online Trading</p>
            </div>
        </div>
        <div class="cell small-0 large-1 medium-1"></div>
    </div>
</template>

<script>
    export default {
        name: "cards"
    }
</script>

<style lang="scss">
    #content {
        height: 280px;
        color: white;

        &_one {
            background-color: #5C213C;
            padding-left: 40px;
            @media screen and (max-width:500px){
                padding-left: 10px;
            }

            button {
                background-color: #DA7D1F;
                border: none;
                color: white;
                padding: 15px 15px;
                text-align: center;
                text-decoration: none;
                display: inline-block;
                font-size: 16px;
                margin: 4px 2px;

                @media screen and (max-width:500px){
                    padding : 5px 5px;
                    font-size: 12px;
                }
            }

            #one {
                padding-top: 40px;
                font-size: 22px;
                font-weight: bolder;
                @media screen and (max-width:500px){
                    padding-top: 16px;
                }
            }

            #two {
                font-size: 16px;
                line-height: 1.1em;
                @media screen and (max-width:500px){
                    font-size: 13px;
                }
            }
        }

        &_two {
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("../assets/mobile.jpeg");
            font-size: 22px;
            font-weight: bolder;
            padding-top: 200px;
            padding-left: 40px;

            @media screen and (max-width:500px){
                padding-top: 100px;
            }
        }
    }
</style>
