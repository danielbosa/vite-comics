<template>
    <main>
        <div class="db-container">
            <div class="footer-links">
                <div>
                    <h5>dc comics</h5>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h5>shop</h5>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div>
                    <h5>dc</h5>
                    <ul>
                        <li><a href="#">Term Of Use</a></li>
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
                <div>
                    <h5>sites</h5>
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
    </main>
</template>

<script>
    export default {
        name: 'FooterTwoComponent',
        // data() {
        //     return{

        //     }
        // },
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

    *{
        @include reset;
    }

    main{
        background-image: url(/public/img/footer-bg.jpg);
    }

    .db-container{
        @include db-container;
        padding: 30px 0 40px 0;
        background-image: url(/public/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: 100%;
        background-size: 50%;
    }

    .footer-links{
        display: flex;
        gap: 30px;
    }

    ul{
        margin: 10px 0 15px 0;
        list-style: none;
    }

    h5{
        color: $light;
        text-transform: uppercase;
        font-weight: 900;
    }

    li{
        a{
        font-size: 10px;
        text-decoration: none;
        color: $secondary;
    }
    }

</style>