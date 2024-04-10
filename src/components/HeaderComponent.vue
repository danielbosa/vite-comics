<template>
    <div>
        <div class="db-container d-flex">
            <div class="logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <ul>
                <li v-for="(item,index) in links" :key="index">
                    <a :href="item.link">{{item.name}}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data() {
            return{
                links:[
                    {
                        name: 'characters',
                        link: '#',
                    },
                    {
                        name: 'comics',
                        link: '#',
                    },
                    {
                        name: 'movies',
                        link: '#',
                    },
                    {
                        name: 'tv',
                        link: '#',
                    },
                    {
                        name: 'games',
                        link: '#',
                    },
                    {
                        name: 'collectibles',
                        link: '#',
                    },
                    {
                        name: 'videos',
                        link: '#',
                    },
                    {
                        name: 'fans',
                        link: '#',
                    },
                    {
                        name: 'news',
                        link: '#',
                    },
                    {
                        name: 'shop',
                        link: '#',
                    },
                ]
            }
        },
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