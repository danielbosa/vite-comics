<!-- component for the FooterOneComponent -->

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

.db-img{
    width: 40px;
}
</style>