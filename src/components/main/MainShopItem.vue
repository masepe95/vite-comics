<script>
export default {
    props: ['shop'],
    methods: {
        getImagePath(img) {
            const url = new URL(`../../assets/img/${img}`, import.meta.url);
            return url.href;
        }
    }
}
</script>

<template>
    <li>
        <img :src="getImagePath(shop.img)" :alt="shop.text">
        <p>{{ shop.text }}</p>
    </li>
</template>

<style scoped>
li {
    display: flex;
    align-items: center;
    cursor: pointer;
}

img {
    max-height: 60px;
    margin-right: 1rem;
}

p {
    font-size: .8rem;
    text-transform: uppercase;
    color: white;
}
</style>