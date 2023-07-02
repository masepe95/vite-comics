<script>
export default {
    props: {
        comic: Object
    }
}
</script>

<template>
    <div class="card">
        <figure>
            <img :src="comic.thumb" :alt="comic.series">
        </figure>
        <h4> {{ comic.series }}</h4>
    </div>
</template>

<style scoped>
.card {
    padding: 0 1rem;
    margin: 2rem 0;
    cursor: pointer;
}

figure {
    height: 175px;
    overflow: hidden;
}

img {
    width: 100%;
    height: 150%;
    object-fit: cover;
    object-position: top center;
}

h4 {
    color: white;
    text-transform: uppercase;
    margin-top: 1rem;
    font-weight: normal;
    font-size: .8rem;
}
</style>