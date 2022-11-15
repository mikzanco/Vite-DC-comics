<script>
export default {
  name: 'AppFooter',

}
</script>

<template>
  <footer>
    
    <div class="sectionone">
        <div class="container ">
        
      </div>
    </div>
      
    <div class="containerBig ">
      
      <div class="sectiontwo">
        <div class="container">
          <h4>Dc comics</h4>
          <span>Character</span>
          <span>Comics</span>
          <span>Movies</span>
          <span>TV</span>
          <span>Games</span>
          <span>Videos</span>
          <span>News</span>
          <h4>Shop</h4>
          <span>Shop DC</span>
          <span>Shop DC Collectibles</span>
          <h4>Dc</h4>
          <span>Terms Of Use</span>
          <span>Pricacy pollicy(New)</span>
          <span>Ad Choise</span>
          <span>Advertising</span>
          <span>Jobs</span>
          <span>Subscriptions</span>
          <span>Talent Workshop</span>
          <span>CPSC Certificates</span>
          <span>Ratings</span>
          <span>Shop Help</span>
          <span>Contact Us</span>
          <h4>Sites</h4>
          <span>DC</span>
          <span>Mad Magazine</span>
          <span>DC Kids</span>
          <span>DC Universe</span>
          <span>DC Power Visa</span>
          </div>
        
      </div>
      <div class="sectionthree">
        <div class="container">
          <div class="button">
          <button class="btn">Sign-up now!</button>
        </div>
        <div class="social">
          <span>Follow Us</span>
          
        </div>
        </div>
        
      </div>
    </div>
  </footer>
</template>


// background-image: url("../assets/img/dc-logo-bg.png")
<style lang="scss" scoped>
  
  footer{
    height: 620px;
    width: 100%;
    background-image: url("../assets/img/footer-bg.jpg");
    color: white;
    .sectionone{
      height: 130px;
      width: 100%;
      background-color: #6288f9;
    }
    .sectiontwo{
      height: 370px;
      width: 100%;
    }
    .sectionthree{
      height: calc(620px - 130px - 370px);
      background-color: #050505;
      justify-content: space-between;
    }
    

  }
</style>