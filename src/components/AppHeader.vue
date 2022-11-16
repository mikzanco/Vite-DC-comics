<script>
export default {
  name: 'AppHeader',
}
</script>

<template>
  <header>

    <div class="container">

      <div>
        <img src="/dc-logo.png" alt="">
      </div>

      <nav>

        <ul>
          <li><a href="#">Character</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">Tv</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Collectibles</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Fans</a></li>
          <li><a href="#">News</a></li>
          <li><a class="active" href="#">Shop</a></li>
        </ul>

      </nav>

    </div>
    
  </header>
</template>



<style lang="scss" scoped>

  @use '../style/partials/variables' as *;
  @use '../style/partials/mixin' as *;

  header{
    height: 95px;
    display: flex;
    width: 100%;
    
    .container{
      justify-content: space-around;
      
      
      img{
      height: 70px;         
      }
      ul{
        display: flex;
        list-style: none;
        a{
          text-decoration: none;
          padding: 10px;
          &:hover,
          &:active{
            padding-bottom: 35px;
            border-bottom: 5px solid $primary-color;
            color: $primary-color;
          }
        }
      }
    }
    
  }
</style>