<template>
        <img class="db-img" :src="image" :alt="shop">
        <div>{{shop}}</div>
</template>

<script>
export default {
    name: 'ShopComponent',
    props: ['shop', 'image']
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
        .db-img{
            width: 40px;
            img{
                width: 100%;
            }
        }
    }
</style>