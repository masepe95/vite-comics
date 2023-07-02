<script>
import HeaderLink from './HeaderLink.vue';

export default {
    props: {
        navbar: Array
    },
    components: { HeaderLink }
}
</script>

<template>
    <nav>
        <ul>
            <HeaderLink v-for="item in navbar" :item="item" />
        </ul>
    </nav>
</template>

<style scoped>
ul {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
}
</style>