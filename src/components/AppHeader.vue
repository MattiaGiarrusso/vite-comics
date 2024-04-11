<script>
  export default {
    name: 'AppHeader'
  }
</script>


<template>
    <header class="container">
        <div>
            <img src="../assets/img/dc-logo.png" alt="DC.alt">
        </div>

        <nav>
            <ul>
                <li>
                    <a href="">link</a>
                </li>
                <li>
                    <a href="" class="active">link</a>
                </li>
                <li>
                    <a href="">link</a>
                </li>
                <li>
                    <a href="">link</a>
                </li>
                <li>
                    <a href="">link</a>
                </li>
                <li>
                    <a href="">link</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">

@use '../style/partials/variables' as *;

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 20px;

    nav {

        ul {
            display: flex;
            gap: 15px;
    
            li {
                list-style: none;
            }
    
            a {
                color:  $color-primary;
                padding: 40px 0;
                
                &.active {
                    color: $color-secondary;
                    border-bottom: 4px solid $color-secondary;
                }
            }
        }

    }

}
</style>