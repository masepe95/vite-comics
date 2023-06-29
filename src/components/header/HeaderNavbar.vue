<script>
import HeaderLink from './HeaderLink.vue';
import { navbar } from '@/assets/data'
export default {
    data() {
        return {
            navbar
        }
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