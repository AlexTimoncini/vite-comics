<script>  
  import HeaderApp from './components/HeaderApp.vue';
  import FooterApp from './components/FooterApp.vue';
  import MainApp from './components/MainApp.vue';
  export default{
    name: 'App',
    components: {
      HeaderApp,
      FooterApp,
      MainApp,
    }
  }
</script>

<template>
  <HeaderApp />
  <MainApp />
  <FooterApp />
</template>

<style lang="scss">
  @import url('./styles/general.scss');
</style>
