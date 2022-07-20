<template>
    <div class="main-background">
        <div class="row col-8 mx-auto pt-5">
            <AlbumList/>
        </div>
    </div>
</template>

<script>
import AlbumList from './AlbumList';
export default {
    components: {
        AlbumList
    },
}
</script>

<style>
.main-background{
    height: 100vh;
    background-color: #1E2D3B;
}
</style>