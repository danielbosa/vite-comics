<template>
  <div>
    <HeaderComponent/>
    <MainComponent/>
    <FooterOneComponent/>
    <FooterTwoComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterOneComponent from './components/FooterOneComponent.vue';
import FooterTwoComponent from './components/FooterTwoComponent.vue';

  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      FooterOneComponent,
      FooterTwoComponent,
    },
    // data(){
    //   return{

    //   }
    // },
    methods: {

    },
  }
</script>

<style lang="scss" scoped>
*{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
</style>