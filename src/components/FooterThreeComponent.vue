<template>
    <main>
        <div class="db-container">
            <div class="cta">
                sign-up now!
            </div>
            <div class="footer-icons">
                <div>follow us</div>
                <div>
                    <a href="">
                        <img src="/img/footer-facebook.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="">
                        <img src="/img/footer-twitter.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="">
                        <img src="/img/footer-youtube.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="">
                        <img src="/img/footer-pinterest.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="">
                        <img src="/img/footer-periscope.png" alt="">
                    </a>
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
        background-color: $darkless;
        font-size: 12px;
    }

    .db-container{
        @include db-container;
        padding: 30px 0;
        display: flex;
        justify-content: space-between;
    }

    .cta{
        border: 3px solid #0c7cec;
        padding: 10px;
        color: white;
        text-transform: uppercase;
        font-weight: bold;
    }

    .footer-icons{
        display: flex;
        align-items: center;
        gap: 20px;
        text-transform: uppercase;
        font-weight: bold;
        color: #0c7cec;
        a{
            display: flex;
            align-items: center;
        }
        img{
            width: 100%;
        }
    }

</style>