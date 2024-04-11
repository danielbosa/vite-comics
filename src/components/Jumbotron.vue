<template>
    <div>
        <img src="/img/jumbotron.jpg" alt="">
    </div>
</template>

<script>
    export default {
        name: 'JumbotronComponent',
    }
</script>

<style lang="scss" scoped>
    div{
        height: 300px;
        overflow: hidden;
        img{
            width: 100%;
            background-repeat: no-repeat;
        }
    }
</style>