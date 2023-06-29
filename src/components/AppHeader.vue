<script>
import HeaderLogo from './header/HeaderLogo.vue'
import HeaderNavbar from './header/HeaderNavbar.vue'

export default {
    components: { HeaderLogo, HeaderNavbar }
}
</script>

<template>
    <header>
        <div class="container">
            <HeaderLogo />
            <HeaderNavbar />
        </div>
    </header>
</template>

<style scoped>
.container {
    display: flex;
    justify-content: space-between;
}
</style>