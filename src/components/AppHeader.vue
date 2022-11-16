<script>
export default {
  name: 'AppHeader',
  data(){
    return{
      menu: [
        {
          text: 'Character',
          href: '#',
          current: false
        },
        {
          text: 'Comics',
          href: '#',
          current: false
        },
        {
          text: 'TV',
          href: '#',
          current: false
        },
        {
          text: 'Movies',
          href: '#',
          current: false
        },
        {
          text: 'Games',
          href: '#',
          current: false
        },
        {
          text: 'Collectibles',
          href: '#',
          current: false
        },
        {
          text: 'Videos',
          href: '#',
          current: false
        },
        {
          text: 'Fans',
          href: '#',
          current: false
        },
        {
          text: 'News',
          href: '#',
          current: false
        },
        {
          text: 'Shop',
          href: '#',
          current: false
        },
      ]
    }
  }
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
          <li
            v-for="(link, index) in menu"
            :key="index"
          ><a :class="{'active': link.current}" :href="link.href">{{link.text}}</a>
          </li>
          
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
      justify-content: space-between;
      
      
      img{
      height: 70px;         
      }
      ul{
        display: flex;
        list-style: none;
        a{
          text-decoration: none;
          font-size: 0.8rem;
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