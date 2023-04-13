<template>
  <HeaderComponent/>
  <ContentComponent/>
  <MainComponent/>
  <FooterTop/>
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import ContentComponent from './components/ContentComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import FooterTop from './components/TopFooter.vue';
  export default {
      name: 'App',
      components: {HeaderComponent, ContentComponent, MainComponent, FooterTop}
  }
</script>

<style lang="scss" scoped>

</style>