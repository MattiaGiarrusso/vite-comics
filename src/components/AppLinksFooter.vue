<script>

export default {
    name: 'AppLinksFooter',
    props: {
        title: String,
        link: Array
    }
  }

</script>

<template>
    <div class="nav-item">

        <h4 class="uppercase">{{ title }}</h4>
        <ul class="ms-pdg-bottom-20">
            <li  v-for="text in navSection.link">
                <a href="">{{ text }}</a>
            </li>
        </ul>

    </div>
</template>

<style scoped lang="scss">

 @use '../style/partials/variables' as *;

</style>