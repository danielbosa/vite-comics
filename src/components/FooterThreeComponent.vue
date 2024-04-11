<template>
    <main>
        <div class="db-container">
            <a class="db-cta" href="#">sign-up now!</a>
            <div class="db-footer-icons">
                <div>follow us</div>
                <div>
                    <a href="#">
                        <img src="/img/footer-facebook.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="#">
                        <img src="/img/footer-twitter.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="#">
                        <img src="/img/footer-youtube.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="#">
                        <img src="/img/footer-pinterest.png" alt="">
                    </a>
                </div>
                <div>
                    <a href="#">
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

    .db-cta{
        text-transform: uppercase;
        font-weight: bold;
        border: 3px solid $accenture;
        padding: 10px;
        text-decoration: none;
        color: $light;
    }

    .db-footer-icons{
        display: flex;
        align-items: center;
        gap: 20px;
        text-transform: uppercase;
        font-weight: bold;
        color: $accenture;
        a{
            display: flex;
            align-items: center;
        }
        img{
            width: 100%;
        }
    }

</style>