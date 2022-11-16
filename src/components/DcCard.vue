<script>
export default {
  name: 'DcCard',
  props:{
    cardImage: String,
    cardTitle: String,
  }

}
</script>

<template>
  <div class="card">
    <img :src="cardImage" :alt="cardTitle">
    <h4>{{cardTitle}}</h4>
  </div>
</template>



<style lang="scss" scoped>

  @use '../style/partials/variables' as *;

  .card{
    flex-basis: 15%;
    min-height: 80px; 
    padding: 15px;
    text-align: center;
     
  }
</style>