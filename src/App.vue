<script>  
  import HeaderApp from './components/HeaderApp.vue';
  import FooterApp from './components/FooterApp.vue';
  export default{
    name: 'App',
    components: {
      HeaderApp,
      FooterApp,
    }
  }
</script>

<template>
  <HeaderApp />
  <FooterApp />
</template>

<style lang="scss">
  @import url('./styles/general.scss');
</style>
