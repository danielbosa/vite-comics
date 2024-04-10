<template>
    <main>
        <div class="db-container">
            <div class="footer-links">
                <div>
                    <h4>dc comics</h4>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h4>shop</h4>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div>
                    <h4>dc</h4>
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
                    <h4>sites</h4>
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
    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }

    main{
        background-image: url(/public/img/footer-bg.jpg);
    }

    .db-container{
        max-width: 80%;
        margin: 0 auto;
        padding: 50px 0;
        background-image: url(/public/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: 100%;
        background-size: 45%;
    }

    .debug{
        border: 2px solid red;
    }

    .footer-links{
        display: flex;
        gap: 30px;
    }

    ul{
        margin: 10px 0 15px 0;
        list-style: none;
    }

    h4{
        color: white;
        text-transform: uppercase;
        font-weight: 900;
    }

    li{
        a{
        font-size: small;
        text-decoration: none;
        color: gray;
    }
    }

</style>