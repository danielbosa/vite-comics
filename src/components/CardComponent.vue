<template>
    <div class="card">
        <div class="db-card-img-container">
            <img class="db-card-img" :src="image" alt="">
        </div>
        <div class="db-card-title text-uppercase ">{{title}}</div>
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
    .db-card-title{
        margin-top: 5px;
        font-size: 12px;
    }
    .db-card-img-container{
        height: 250px;
    }
}

.db-card-img{
        width: 100%;
        height: 100%;
        object-fit: fill;
    }
</style>