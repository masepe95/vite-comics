<script>
import MainComicsContainer from './MainComicsContainer.vue';

export default {
    components: { MainComicsContainer }
}
</script>

<template>
    <section id="jumbotron">
        <figure>
            <img src="@/assets/img/jumbotron.jpg" alt="jumbotron">
        </figure>
    </section>
    <section id="content">
        <MainComicsContainer />
    </section>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

#content {
    background-color: $dark_gray;

    #jumbotron {
        height: 400px;
        overflow: hidden;
    }

    .container {
        height: 100%;
        display: flex;
        align-items: center;
    }
}

h2 {
    font-size: 2.5rem;
    color: white;
    margin: 4rem 0;
}
</style>