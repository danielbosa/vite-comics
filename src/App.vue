<template>
  <div>
    <HeaderComponent/>
    <JumbotronComponent/>
    <MainComponent/>
    <FooterOneComponent/>
    <FooterTwoComponent/>
    <FooterThreeComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import JumbotronComponent from './components/Jumbotron.vue';
import MainComponent from './components/MainComponent.vue';
import FooterOneComponent from './components/FooterOneComponent.vue';
import FooterTwoComponent from './components/FooterTwoComponent.vue';
import FooterThreeComponent from './components/FooterThreeComponent.vue';

  export default {
    name: 'App',
    components: {
      HeaderComponent,
      JumbotronComponent,
      MainComponent,
      FooterOneComponent,
      FooterTwoComponent,
      FooterThreeComponent,
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

</style>