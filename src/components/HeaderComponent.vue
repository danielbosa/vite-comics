<template>
    <div>
        <div class="db-container db-d-flex">
            <div class="db-logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <ul>
                <li v-for="(item,index) in items" :key="index">
                    <a :href="item.link">{{item.name}}</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import {headerOptions} from '../data/store.js';
    export default {
        name: 'HeaderComponent',
        data() {
            return{
                items: headerOptions,
            }
        },
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

    .db-container{
        @include db-container;
        height: 100px;
    }

    .db-d-flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .db-logo{
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
                font-size: 12px;
                line-height: 100px;
            }
        }
    }
</style>