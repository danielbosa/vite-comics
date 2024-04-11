<template>
    <div>
        <div class="db-container">
            <div>--> Content goes here <--</div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainComponent',
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
            padding: 30px 0;
        }
    }
</style>