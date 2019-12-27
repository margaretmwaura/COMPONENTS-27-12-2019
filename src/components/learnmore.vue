
<template>
    <div id="events" class="grid-frame">
        <div class="grid-container">
        <div class="grid-x">
            <div class="cell medium-5 large-5 small-5"></div>
            <div class="cell medium-2 large-2 small-2">
                <button @click="ok"> Find out more</button>
                <slot></slot>
            </div>
            <div class="cell medium-5 large-5 small-5"></div>

        </div>
        </div>
    </div>
</template>
<script>
    export default
    {
        name: "learnmore",
        methods: {
            ok() {
                this.$emit('finished')
            }
        }
    }
</script>
<style lang="scss">
#events
{
    height: 100px;
    button {
        background-color: #5C213C;
        border: none;
        color: white;
        padding: 15px 15px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        margin: 4px 2px 0px 20px;
        position:relative;

    }
}
</style>
