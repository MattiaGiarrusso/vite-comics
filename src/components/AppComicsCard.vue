<script>
  export default {
    name: 'AppComicsCard',
    props: ['thumb','series']
  }
</script>

<template>
  
  <div class="comics-card">
    <a class="uppercase" href="">
      
      <div class="comic-container">
        <img :src="thumb" alt="">
      </div>
      
      <figcaption>{{ series }}</figcaption>
      
    </a>    

  </div>

</template>

<style scoped lang="scss">
  @use '../style/partials/variables' as *;

  .comics-card {
    width: calc(100% / 6);
    display: flex;
    flex-direction: column;
    padding: 10px 10px;
    &:hover {
      opacity: 0.6;
    }
    
    a {
      color: white;
      font-weight: 400;
    }

    .comic-container {
      margin-bottom: 10px;

    } 
      
        
      img {
          width: 100%;
          height: 200px;
      }


      figcaption {
        align-self: flex-start;
      }

  }

</style>