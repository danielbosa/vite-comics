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
    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }

    .db-container{
        max-width: 80%;
        height: 100px;
        margin: 0 auto;
    }

    .debug{
        border: 2px solid red;
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
                    color: #0c7cec;
            }
            &:hover{
                border-bottom: 4px solid #0c7cec;
            }

            a{
                text-decoration: none;
                color: black;
                font-weight: 900;
                font-size: 10px;
                line-height: 100px;
            }
        }
    }
</style>