<script>
  export default {
    name: 'AppSectionLinks'
  }
</script>

<template>

  <section class="container">

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

</template>

<style scoped lang="scss">

  @use '../style/partials/variables' as *;

  section {
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

  

</style>
