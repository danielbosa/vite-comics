<template>
    <main>
        <div class="db-container">
            <div class="db-footer-links">
                <div>
                    <FooterMenuComponent v-for="(item,index) in menu.slice(0,2)" :key="index" :menuItem="item"/>
                </div>
                <div>
                    <FooterMenuComponent v-for="(item,index) in menu.slice(2,3)" :key="index" :menuItem="item"/>
                </div>
                <div>
                    <FooterMenuComponent v-for="(item,index) in menu.slice(3)" :key="index" :menuItem="item"/>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import {footerMenu} from '../data/store.js';
import FooterMenuComponent from './FooterMenuComponent.vue';
    export default {
        name: 'FooterTwoComponent',
        components:{
            FooterMenuComponent
        },
        data() {
            return{
                menu: footerMenu
            }
        },
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

    *{
        @include reset;
    }

    main{
        background-image: url(/public/img/footer-bg.jpg);
    }

    .db-container{
        @include db-container;
        padding: 30px 0 40px 0;
        background-image: url(/public/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: 100%;
        background-size: 50%;
    }

    .db-footer-links{
        display: flex;
        gap: 30px;
    }

</style>