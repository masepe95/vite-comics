<script>
import MainComic from './MainComic.vue';
export default {
    components: { MainComic },
    props: {
        comics: Array
    }
}

</script>




<template>
    <div class="container">

        <div class="flex-container">
            <MainComic v-for="comic in comics" :comic="comic" />
        </div>
    </div>
</template>




<style lang="scss" scoped>
.flex-container {

    display: flex;

    justify-content: center;

    flex-wrap: wrap;




    .card {
        flex: 0 0 calc(100% / 6);
    }

}
</style>