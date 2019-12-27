
<template>
    <div>
        <button @click="ok"> Click me</button>
        <slot></slot>
    <h1>I am Maggie , I am really trying man</h1>
    <buttonmine></buttonmine>

    </div>
</template>


<script>
    import buttonmine from './button'
    export default
    {
        name: "pratice",
        components: {
           buttonmine
        },
        methods: {
            ok() {
                this.$emit('finished')
            }
        }
    }
</script>

<style scoped>

</style>
