<script>
export default {
}
</script>

<template>
    <section id="jumbo">
        <div class="container">
            <div class="lists">
                <div class="list">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h4>SHOP</h4>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="list">
                    <h4>DC</h4>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="list">
                    <h4>SITES</h4>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '@/assets/scss/vars' as *;

#jumbo {
    background-image: url('@/assets/img/dc-logo-bg.png'), url("@/assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: 40%, cover;
    background-position: 80%, center;
    padding: 4rem 0;
}

.lists {
    display: flex;
    align-items: start;
}

.list {
    min-width: 155px;
    margin-right: 1.5rem;
}

h4 {
    font-family: $secondary_font;
    color: white;
    margin-top: 1rem;
    font-weight: 900;
    font-size: 1.8rem;
}

a {
    color: gray;
}
</style>