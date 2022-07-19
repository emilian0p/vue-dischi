<template>
    <main>
        <AlbumContainer />
    </main>
</template>

<script>
import AlbumContainer from './AlbumContainer.vue';

export default {

    components: {
        AlbumContainer,
    },
}
</script>

<style lang="scss">
main {
    height: 90vh;
    background-color: #1f2d3b;
}
</style>