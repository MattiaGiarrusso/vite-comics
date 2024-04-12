<script>
  export default {
    name: 'AppFooter'
  }
</script>



<template>

  <section id="footer-link" class="container">

    <nav>
      <div class="nav-item">

        <h4>DC COMICS</h4>
          <ul class="ms-pdg-20">
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
          </ul>
          
          <h4>SHOP</h4>
          <ul>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
          </ul>
          
        </div>

        <div class="nav-item">

          <h4>DC</h4>
          <ul>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
            <li>
              <a href="">Link</a>
            </li>
          </ul>

        </div>

        <div class="nav-item">

          <h4>SITES</h4>
            <ul>
              <li>
                <a href="">Link</a>
              </li>
              <li>
                <a href="">Link</a>
              </li>
              <li>
                <a href="">Link</a>
              </li>
              <li>
                <a href="">Link</a>
              </li>
              <li>
                <a href="">Link</a>
              </li>
            </ul>

        </div>

    </nav>


    <div class="img-container">

    </div>
    
  </section>

  <section id="footer-bottom" class="container">

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

  #footer-link {
    height: 340px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    color: antiquewhite;
    display: flex;
    justify-content: space-between;
    padding: 0px 150px;

    >* {
      width: 50%;
    }
    
    .img-container {      
      background-image: url('../assets/img/dc-logo-bg.png');
      background-repeat: no-repeat;
      background-size: cover;
      background-position: center;
      padding: 0;
    }
    
    nav {
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
      padding-top: 40px;

      a {
            font-size: 10px;
            font-weight: 500;
            color: lightgray;
          }

    }
       
  
  }

  #footer-bottom {
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
