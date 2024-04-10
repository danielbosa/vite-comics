<template>
    <div>
        <div class="db-container">
            <ul>
                <li v-for="(item,index) in shops" :key="index">
                    <img class="img" :src="item.path" :alt="item.path">
                    <div>{{item.name}}</div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterOneComponent',
        data() {
            return{
                shops: [
                    {
                    name: 'digital comics',
                    path: '/public/img/buy-comics-digital-comics.png',
                    },
                    {
                    name: 'digital comics',
                    path: '/public/img/buy-comics-merchandise.png',
                    },
                    {
                    name: 'digital comics',
                    path: '/public/img/buy-comics-subscriptions.png',
                    },
                    {
                    name: 'digital comics',
                    path: '/public/img/buy-comics-shop-locator.png',
                    },
                    {
                    name: 'digital comics',
                    path: '/public/img/buy-dc-power-visa.svg',
                    }]
            }
        },
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;

    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        background-color: $accenture;
    }

    .db-container{
        max-width: 80%;
        margin: 0 auto;
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
        color: $light;
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