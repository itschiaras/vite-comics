<template>
  <HeaderComponent/>
  <ContentComponent/>
  <MainComponent/>
  <FooterTop/>
  <FooterBottom/>
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import ContentComponent from './components/ContentComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import FooterTop from './components/TopFooter.vue';
  import FooterBottom from './components/BottomFooter.vue';
  export default {
      name: 'App',
      components: {HeaderComponent, ContentComponent, MainComponent, FooterTop, FooterBottom}
  }
</script>

<style lang="scss" scoped>
  
</style>