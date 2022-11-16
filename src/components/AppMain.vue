<script> 

  import DcCard from './DcCard.vue';

  import dcComics from '../data/dcComics'

export default {
    name: 'AppMain',
    components:{
      DcCard
    },
    data(){
      return{
        dcComics
      }
    }
}
</script>

<template>
  <main>    
    <div class="jumbotron">
      <!-- <img src="" alt=""> -->
    </div>
    <div class="container cards">
      <DcCard
        v-for="(card, index) in dcComics"
        :key="index"
        :cardImage="card.thumb"
        :cardTitle="card.series"
        />
    </div>

  </main>
</template>



<style lang="scss" scoped>

  @use '../style/partials/variables' as *;


  main{
    
    width: 100%;
    background-color: $secondary-color; 
    color: white;
    .container{
      width: 100%;
    }
    .jumbotron{
      height: 400px;
      width: 100%;
      background-image: url("../assets/img/jumbotron.jpg");
    }
    .cards{
      display: flex;
      flex-wrap: wrap;
    }
  }
</style>