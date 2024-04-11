<!-- component for the FooterTwoComponent: menu in the footer -->
<template>
    <h5>{{ menuItem.title }}</h5>
        <ul>
            <li v-for="(item,index) in menuItem.links" :key="index">
                <a :href="item.url">{{item.text}}</a>
            </li>
        </ul>
</template>

<script>
export default {
    name: 'FooterMenuComponent',
    props: {
        menuItem: Object
    }
}
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
@use '/src/assets/styles/partials/mixin' as *;

    ul{
        margin: 10px 0 15px 0;
        padding: 0;
        list-style: none;
    }

    h5{
        color: $light;
        text-transform: uppercase;
        font-weight: 900;
    }

    li{
        a{
        font-size: 12px;
        text-decoration: none;
        color: $secondary;
    }
}

</style>