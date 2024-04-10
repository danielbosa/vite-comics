<template>
    <div>
        <div class="db-container d-flex">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <ul>
                <li><a href="#">characters</a></li>
                <li><a href="#">comics</a></li>
                <li><a href="#">movies</a></li>
                <li><a href="#">tv</a></li>
                <li><a href="#">games</a></li>
                <li><a href="#">collectibles</a></li>
                <li><a href="#">videos</a></li>
                <li><a href="#">fans</a></li>
                <li><a href="#">news</a></li>
                <li><a href="#">shop</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HeaderComponent',
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
        @include reset
    }

    .db-container{
        @include db-container;
        height: 100px;
    }

    .d-flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .logo{
        width: 100px;
        img{
            width: 100%;
            padding: 5px;
        }
    }

    ul{
        list-style: none;
        display: flex;
        padding: 0;
        margin: 0;

        li{
            height: 100px;
            margin: 0px 10px;
            text-transform: uppercase;
            &:hover a{
                    color: $accenture;
            }
            &:hover{
                border-bottom: 4px solid $accenture;
            }

            a{
                text-decoration: none;
                color: $darkest;
                font-weight: 900;
                font-size: 10px;
                line-height: 100px;
            }
        }
    }
</style>