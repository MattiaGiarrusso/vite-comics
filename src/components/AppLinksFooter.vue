<script>

export default {
    name: 'AppLinksFooter',
    data () {
        return {
            navSections: [
                {
                    title: 'Dc Comics',
                    link: ['Characters','Comics','Movies','TV','Games','Videos','News',]
                },

                {
                    title: 'Shop',
                    link: ['Shop DC','Shop DC Collectibles',]
                },

                {
                    title: 'DC',
                    link: ['Terms of Use','Privacy policy (New)','Ad Choices','Advertising','Jobs','Subscriptions','Talent Workshops','CPSC Certificates','Ratings','Shop Help','Contact Us',]
                },

                {
                    title: 'Sites',
                    link: ['DC','MAD Magazines','DC Kids','DC Universe','DC Power Visa',]
                },
            ]
        }
      }
  }

</script>

<template>
    <div class="nav-item" v-for="navSection in navSections">

        <h4 class="uppercase">{{ navSection.title }}</h4>
        <ul class="ms-pdg-bottom-16">
            <li v-for="text in navSection.link">
                <a href="#" :alt="text">{{ text }}</a>
            </li>
        </ul>

    </div>
</template>

<style scoped lang="scss">

 @use '../style/partials/variables' as *;

 a {
    font-size: 10px;
    font-weight: 500;
    color: lightgray;

    &:hover {
        color: $color-secondary;
    }
 }

</style>