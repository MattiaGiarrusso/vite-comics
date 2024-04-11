<script>
  export default {
    name: 'AppFooter'
  }
</script>

<template>
    <section class="container">
        <div class="footer-left">
            <button>SIGN-UP NOW!</button>
        </div>

        <div class="footer-right">
            <span>FOLLOW US</span>

            <div class="social-icon">
                <img src="../assets/img/footer-facebook.png" alt="">                
            </div>
            <div class="social-icon">
                <img src="../assets/img/footer-twitter.png" alt="">                
            </div>
            <div class="social-icon">
                <img src="../assets/img/footer-youtube.png" alt="">                
            </div>
            <div class="social-icon">
                <img src="../assets/img/footer-pinterest.png" alt="">                
            </div>
            <div class="social-icon">
                <img src="../assets/img/footer-periscope.png" alt="">                
            </div>
        </div>        

    </section>
</template>

<style scoped lang="scss">

    @use '../style/partials/variables' as *;

    section {
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: $color-primary;

        .footer-right {
            color: $color-secondary;
            display: flex;
            align-items: center;
            gap: 16px;
        }

        button {
            background-color: transparent;
            border: 2px solid $color-secondary;
            padding: 8px 12px;
            color: white;
            font-weight: 700;
            cursor: pointer;

            &:hover {
                background-color: $color-secondary;
                transition: 0.2s; 
            }
        }
    }

    

</style>