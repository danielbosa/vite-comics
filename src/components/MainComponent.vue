<template>
    <div>
        <div class="">
            <div class="db-container container py-5">
                <div class="row g-3">
                    <div class="col-4 col-md-3 col-lg-2" v-for="(item,index) in items" :key="index">
                        <CardComponent :image="item.thumb" :title="item.series"/>
                    </div>
                </div>
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
            font-weight: 900;
        }
    }
    
</style>