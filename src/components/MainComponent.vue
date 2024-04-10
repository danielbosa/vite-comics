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
    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        background-color: black;
    }

    .db-container{
        max-width: 80%;
        margin: 0 auto;
        div{
            color: white;
            font-weight: 900;
            padding: 30px 0;
        }
    }

    .debug{
        border: 2px solid red;
    }
</style>