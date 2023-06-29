<script>
export default {
}
</script>

<template>
    <section id="content">
        <div class="container">
            <h2>Content goes here</h2>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

#content {
    background-color: $dark_gray;

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