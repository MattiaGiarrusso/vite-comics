<script>
  export default {
    name: 'AppMainBlue'
  }
</script>

<template>
    <section class="container">
        <ul>
            <li>
                <img src="" alt="">
                <a href="">link</a>
            </li>
            <li>
                <img src="" alt="">
                <a href="">link</a>
            </li>
            <li>
                <img src="" alt="">
                <a href="">link</a>
            </li>
            <li>
                <img src="" alt="">
                <a href="">link</a>
            </li>
            <li>
                <img src="" alt="">
                <a href="">link</a>
            </li>
        </ul>
    </section>
</template>

<style scoped lang="scss">

@use '../style/partials/variables' as *;

section {
    height: 140px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: $color-secondary;
    color: white;

    ul {
        display: flex;
        gap: 20px;

        a {
            color: white;
            font-weight: 300;
        }
    }
    
    
}

</style>