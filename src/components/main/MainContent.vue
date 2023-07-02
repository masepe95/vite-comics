<script>
import MainComicsContainer from './MainComicsContainer.vue';

export default {
    components: { MainComicsContainer },
    props: {
        comics: Array
    }
}
</script>

<template>
    <section id="jumbotron">
        <figure>
            <img src="@/assets/img/jumbotron.jpg" alt="jumbotron">
        </figure>
    </section>
    <section id="content">
        <MainComicsContainer :comics="comics" />
    </section>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

#jumbotron {
    height: 400px;
    overflow: hidden;
}

#content {
    background-color: $dark_gray;
    position: relative;
    padding-bottom: 3rem;
}

h2 {
    font-size: 2.5rem;
    color: white;
    margin: 4rem 0;
}
</style>