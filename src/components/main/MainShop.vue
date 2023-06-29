<script>
import MainShopItem from './MainShopItem.vue';

export default {
    components: { MainShopItem },
    data() {
        return {
            shops: [
                {
                    text: 'Digital Comics',
                    img: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'DC Merchandise',
                    img: 'buy-comics-merchandise.png'
                },
                {
                    text: 'Subscription',
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'Comic Shop Locator',
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'DC Power Visa',
                    img: 'buy-dc-power-visa.svg'
                },
            ]
        }
    }
}
</script>

<template>
    <section id="shop">
        <div class="container">
            <ul>
                <MainShopItem v-for:="shop in shops" :shop="shop" />
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

#shop {
    background-color: $dc-blue;
}

ul {
    height: 100%;
    display: flex;
    align-items: center;

    li {
        flex: 0 0 20%;
        margin: 3rem 0;
    }
}
</style>