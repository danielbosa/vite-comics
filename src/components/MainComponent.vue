<template>
    <div>
        <div class="">
            <div class="container py-5">
                <div class="row gx-5 gy-5">
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                    <div class="col-4 col-md-3 col-lg-2">
                        <CardComponent/>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
</template>

<script>
import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
      CardComponent
    },
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
        @include reset;
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