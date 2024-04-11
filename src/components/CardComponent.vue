<template>
    <div class="card">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <div class="db-card-title">TITOLO</div>

        <img :src="image" alt="">
        <div class="db-card-title">TITOLO</div>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ['image','title']
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

.card{
    --bs-card-bg: transparent;
    .db-card-title{
        margin-top: 5px;
    }
}
</style>