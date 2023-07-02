<script>
import MainContent from './main/MainContent.vue';
import MainShop from './main/MainShop.vue';

export default {
    components: { MainContent, MainShop },
    props: {
        comics: Array
    }
}
</script>

<template>
    <main>
        <MainContent :comics="comics" />
        <MainShop />
    </main>
</template>

<style scoped></style>