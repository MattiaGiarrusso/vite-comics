<script>
  export default {
    name: 'AppMainContent'
  }
</script>

<template>
    <section class="container">
        <div>
            <span>--> Content goes here <-- </span>
        </div>
    </section>
</template>

<style scoped lang="scss">

@use '../style/partials/variables' as *;

section {
    height: 100px;
    display: flex;
    align-items: center;
    background-color: black;
    color: white;
}

</style>