<template>
    <main>
        <div class="db-container">
            <div class="cta">
                sign-up now!
            </div>
            <div class="footer-icons">
                <div>follow us</div>
                <div>
                    <img src="/public/img/footer-facebook.png" alt="">
                </div>
                <div>
                    <img src="/public/img/footer-twitter.png" alt="">
                </div>
                <div>
                    <img src="/public/img/footer-youtube.png" alt="">
                </div>
                <div>
                    <img src="/public/img/footer-pinterest.png" alt="">
                </div>
                <div>
                    <img src="/public/img/footer-periscope.png" alt="">
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
        background-color: #303030;
        font-size: small;
    }

    .db-container{
        max-width: 80%;
        margin: 0 auto;
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
        gap: 10px;
        text-transform: uppercase;
        font-weight: bold;
        color: #0c7cec;
        i{
            background-color: #797979;
            color: transparent;
        };
        img{
            width: 30px;
        }
    }

</style>