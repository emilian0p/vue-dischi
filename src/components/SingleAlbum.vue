<template>
    <div class="albums">
        <div>
            <img src="" alt="title">
        </div>
        <h2> titolo </h2>
        <p>autore</p>
        <span>anno</span>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap.scss";

.albums {
        background-color: #2E3A46;
        width: calc((100% / 5) - 2rem);
        text-align: center;
}
</style>