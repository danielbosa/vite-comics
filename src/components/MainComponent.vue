<template>
    <div>
        <div class="db-container pb-4">
            <div class="container py-5">
                <div class="row g-3">
                    <div class="col-4 col-md-3 col-lg-2 h-100" v-for="(item,index) in items" :key="index">
                        <CardComponent :image="item.thumb" :title="item.series"/>
                    </div>
                </div>
            </div>
            <div class="text-center">
                <button class="db-btn">Load more</button>
            </div>    
        </div>
    </div>
    
</template>

<script>
import {comics} from '../data/store.js';
import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
      CardComponent
    },
        data() {
            return{
                items: comics
            }
        },
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

    *{
        background-color: $darkest;
    }
    
    .db-container{
        @include db-container;
        div{
            color: $light;
        }
    }

    .db-btn{
        padding: 5px 50px;
        background-color: $accenture;
        color: $light;
        text-transform: uppercase;
        font-weight: bold;
    }
    
</style>