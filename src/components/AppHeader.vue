<script>
import HeaderLogo from './header/HeaderLogo.vue'
import HeaderNavbar from './header/HeaderNavbar.vue'

export default {
    props: {
        navbar: Array
    },
    components: { HeaderLogo, HeaderNavbar }
}
</script>

<template>
    <header>
        <div class="container">
            <HeaderLogo />
            <HeaderNavbar :navbar="navbar" />
        </div>
    </header>
</template>

<style scoped>
header {
    position: sticky;
    top: 0;
    left: 0;
    background-color: white;
}

.container {
    display: flex;
    justify-content: space-between;
}
</style>