<template>
  <HeaderComponent/>
  <ContentComponent/>
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import ContentComponent from './components/ContentComponent.vue';
  export default {
      name: 'App',
      components: {HeaderComponent, ContentComponent}
  }
</script>

<style lang="scss" scoped>

</style>