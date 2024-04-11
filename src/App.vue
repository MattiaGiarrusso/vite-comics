<script>
  import AppHeader from './components/AppHeader.vue';
  import AppSectionContent from './components/AppSectionContent.vue';
  import AppSectionBlue from './components/AppSectionBlue.vue';
  import AppSectionLinks from './components/AppSectionLinks.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
    components: {
      AppHeader,
      AppSectionContent,
      AppSectionBlue,
      AppSectionLinks,
      AppFooter
    }
  }
</script>

<template>
  <AppHeader></AppHeader>

  <main>
    <AppSectionContent></AppSectionContent>
    <AppSectionBlue></AppSectionBlue>
    <AppSectionLinks></AppSectionLinks>
    <AppFooter></AppFooter>
  </main>
</template>

<style lang="scss">

  @use './style/generic';
  @use './style/partials/variables' as *;

</style>
