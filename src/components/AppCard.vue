<script>
export default {
    props: {
        comicsEdition: Object
    }
}
</script>

<template>
    <div class="card-content">
        <div class="img-container">
            <img :src="comicsEdition.thumb" :alt="comicsEdition.series">
        </div>
        <h4>{{ comicsEdition.series }}</h4>
    </div>
</template>

<style lang="scss" scoped>
.card-content {
    padding: 25px 0px;
    margin: 10px;
    width: calc(100% / 6 - 20px);
    height: 310px;
}

img {
    width: 100%;
    aspect-ratio: 3/4;
    object-fit: cover;
}

h4 {
    text-transform: uppercase;
    color: #fff;
    margin-top: 6px;
}
</style>