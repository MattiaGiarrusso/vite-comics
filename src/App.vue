<script>
  import AppHeader from './components/AppHeader.vue';
  import AppSectionContent from './components/AppSectionContent.vue';
  import AppSectionBlue from './components/AppSectionBlue.vue';
  import AppSectionLinks from './components/AppSectionLinks.vue';

  export default {
    components: {
      AppHeader,
      AppSectionContent,
      AppSectionBlue,
      AppSectionLinks,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>

  <main>
    <AppSectionContent></AppSectionContent>
    <AppSectionBlue></AppSectionBlue>
    <AppSectionLinks></AppSectionLinks>
  </main>
</template>

<style lang="scss">

  @use './style/generic';

</style>
