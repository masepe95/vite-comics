<script>
export default {
    props: ["item"],
    computed: {
        capitalizedText() {
            return this.item.text.toUpperCase();
        }
    }
}
</script>

<template>
    <li><a :class="{ 'current': item.current }" :href="item.url">{{ capitalizedText
    }}</a>
    </li>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

a {
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: $secondary_font;
    font-weight: 700;
    color: $gray;
    padding: 0 .5rem
}

li,
a {
    height: 100%;
}

li {
    padding: 0 .25rem;
}

.current {
    border-top: 5px solid transparent;
    border-bottom: 5px solid $dc_blue;
}
</style>