<template>
    <div class="card">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <div class="card-body">
            <p class="card-text">TITOLO</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

*{
        @include reset
    }



</style>