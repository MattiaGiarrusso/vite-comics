<script>
  export default {
    name: 'AppMainBlue',
    data () {
        return {
            links: [
                {
                    icon: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    icon: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    icon: 'buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    icon: 'buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTIONS'
                },                
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL('../assets/img/' + name, import.meta.url).href;
        }
    }
  }
</script>

<template>
    <section class="container">
        <ul class="ms-gap-40">
            <li v-for="link in links">
                <img :src="getImageUrl(link.icon)" class="ms-pdg-right-10" :alt="link.text">
                <a href="">{{ link.text }}</a>
            </li>
        </ul>
    </section>
</template>

<style scoped lang="scss">

@use '../style/partials/variables' as *;

section {
    height: 120px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: $color-secondary;
    color: white;

    ul {
        display: flex;

        li {
            display: flex;
            align-items: center;

            img {
                width: 40px;
            }
    
            a {
                color: white;
                font-weight: 300;
            }
        }

    }    
    
}

</style>