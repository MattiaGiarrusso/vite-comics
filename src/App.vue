<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMainContent from './components/AppMainContent.vue';
  import AppMainBlue from './components/AppMainBlue.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppMainBlue,
      AppFooter,
    },
  }
</script>

<template>
  <AppHeader></AppHeader>

  <main>
    <AppMainContent></AppMainContent>
    <AppMainBlue></AppMainBlue>
  </main>

  <footer>
    <AppFooter></AppFooter>
  </footer>
</template>

<style lang="scss">

  @use './style/generic';

</style>
