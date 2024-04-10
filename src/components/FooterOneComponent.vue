<template>
    <div>
        <div class="db-container">
            <ul>
                <li>
                    <div class="img">
                        <img src="/public/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div>digital comics</div>
                </li>
                <li>
                    <div class="img">
                        <img src="/public/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div>dc merchandise</div>
                </li>
                <li>
                    <div class="img">
                        <img src="/public/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div>subscription</div>
                </li>
                <li>
                    <div class="img">
                        <img src="/public/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div>comic shop locator</div>
                </li>
                <li>
                    <div class="img">
                        <img src="/public/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div>dc power visa</div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterOneComponent',
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
        background-color: #009FE0;
    }

    .db-container{
        max-width: 80%;
        margin: 0 auto;
    }

    .debug{
        border: 2px solid red;
    }

    ul{
        padding: 50px 0;
        display: flex;
        justify-content: space-around;
    }

    li{
        display: flex;
        align-items: center;
        gap: 10px;
        color: white;
        text-transform: uppercase;
        font-size:x-small;
        .img{
            width: 40px;
            img{
                width: 100%;
            }
        }
    }
</style>