<script>
import FooterSignupButton from './FooterSignupButton.vue';

export default {
    components: { FooterSignupButton }
}
</script>

<template>
    <div class="footer-bottom">
        <div class="container">
            <div class="flex-cont">
                <FooterSignupButton />
                <div class="social-icons">
                    <div class="follow-us">
                        FOLLOW US
                    </div>
                    <div class="icons">
                        <a href="#">
                            <img src="@/assets/img/footer-facebook.png" alt="facebook">
                        </a>
                        <a href="#">
                            <img src="@/assets/img/footer-twitter.png" alt="twitter">
                        </a>
                        <a href="#">
                            <img src="@/assets/img/footer-youtube.png" alt="youtube">
                        </a>
                        <a href="#">
                            <img src="@/assets/img/footer-pinterest.png" alt="pinterest">
                        </a>
                        <a href="#">
                            <img src="@/assets/img/footer-periscope.png" alt="periscope">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

.footer-bottom {
    background-color: $gray;
    padding: 2rem 0;
    position: sticky;
    bottom: 0;
    left: 0;
    right: 0;
}

.flex-cont {
    display: flex;
    justify-content: space-between;
}

.social-icons {
    display: flex;
    align-items: center;

    .follow-us {
        color: $dc-blue;
        font-weight: 900;
    }

    .icons {
        display: flex;

        img {
            margin-left: 1.5rem;
        }
    }

}
</style>