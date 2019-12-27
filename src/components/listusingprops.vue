<template>
    <div>
        <h1>Vue Top 20 Artists</h1>
        <ul>
            <li v-for="artist in artists" :key="artist.id">
                <h3>{{artist.name}}</h3>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "listusingprops",
        props:['artists']
    }
</script>

<style scoped>

</style>
