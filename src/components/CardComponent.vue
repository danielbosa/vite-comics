<template>
    <div class="card">
        <img :src="image" alt="">
        <div class="db-card-title">{{title}}</div>
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