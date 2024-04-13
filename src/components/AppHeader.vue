<script>
  export default {
    name: 'AppHeader',
    data () {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                },
                {
                    text: 'COMICS',
                },
                {
                    text: 'MOVIES',
                },
                {
                    text: 'TV',

                },
                {
                    text: 'GAMES',

                },
                {
                    text: 'COLLECTIBLES',
                },
                {
                    text: 'VIDEOS',

                },
                {
                    text: 'FANS',

                },
                {
                    text: 'NEWS',

                },
                {
                    text: 'SHOP',
                },
            ],
            activeLink: null,
        }
    },
    methods: {
        ActiveIndexLink(index) {
        this.activeLink = index;
      },
    }
  }
</script>


<template>
    <header class="container">
        <div>
            <img src="../assets/img/dc-logo.png" alt="DC.alt">
        </div>

        <nav>
            <ul>
                <li v-for="link in links" @click="ActiveIndexLink(link)">
                    <a :class="{'active': link == activeLink}"  href="#">{{ link.text }}</a>
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
    height: 80px;
    padding-top: 8px;
    padding-bottom: 8px;

    div {
        height: 100%;

        img {
            height: 100%;;
        }
    }

    nav {

        ul {
            display: flex;
            gap: 18px;
            
            a {
                font-size: 12px;
                color: $color-primary;
                padding: 26px 0;

                &.active {
                    color: $color-secondary;
                    border-bottom: 4px solid $color-secondary;
                }
            }

        }
    
    }

}

</style>