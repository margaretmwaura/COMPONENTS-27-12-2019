<template>
    <div class="grid-frame">
        <div class="grid-frame">
            <div class="grid-x grid-margin-x">
                <div class="cell medium-6 large-6 small-6">
                 <cards/>
                </div>
                <div class="cell medium-6 large-6 small-6">
                 <cards/>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import cards from './cards'
    export default {
        name: "tabslayout",
        components: {
            cards
        }
    }
</script>

<style lang="scss">

</style>
