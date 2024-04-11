<template>
    <div>
        <div class="db-container">
            <ul>
                <li v-for="(item,index) in items" :key="index">
                    <ShopComponent :image="item.path" :shop="item.name"/>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import {shops} from '../data/store.js';
import ShopComponent from './ShopComponent.vue';
    export default {
        name: 'FooterOneComponent',
        components:{
            ShopComponent
        },
        data(){
            return{
                items: shops
        }
    },
}
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

    *{
        @include reset;
        background-color: $accenture;
    }

    .db-container{
        @include db-container
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
        font-size: 12px;
    }
</style>