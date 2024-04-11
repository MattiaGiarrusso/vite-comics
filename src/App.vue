<script>
  import AppHeader from './components/AppHeader.vue';
  import AppSectionContent from './components/AppSectionContent.vue';
  import AppSectionBlue from './components/AppSectionBlue.vue';

  export default {
    components: {
      AppHeader,
      AppSectionContent,
      AppSectionBlue,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>

  <main>
    <AppSectionContent></AppSectionContent>
    <AppSectionBlue></AppSectionBlue>
  </main>
</template>

<style lang="scss">

  @use './style/generic';

</style>
