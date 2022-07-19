<template>
    <div class="container">
         <SingleAlbum />
    </div>
</template>

<script>
import SingleAlbum from './SingleAlbum.vue';
export default {
    components: {
        SingleAlbum,
    },
}
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap.scss';

div.container {
    width: 60%;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
}
</style>