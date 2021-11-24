<template>
  <div class="container-shop fc-flex-align-center">
   <div class="fc-container">
     <ul class="fc-flex-between-align-center">

       <li>
          <div class="icon-shop">
             <img src="../assets\img\buy-comics-digital-comics.png" alt="digital-comics">
          </div>
          <span>DIGITAL COMICS</span>        
       </li>
    
       <li>
          <div class="icon-shop">
             <img src="../assets\img\buy-comics-merchandise.png" alt="digital-comics">
          </div>
          <span>DC MERCHANDISE</span>        
       </li>
    
       <li>
          <div class="icon-shop">
             <img src="../assets\img\buy-comics-subscriptions.png" alt="digital-comics">
          </div>
          <span>SUBSCRIPTION</span>        
       </li>
    
       <li>
          <div class="icon-shop">
             <img src="../assets\img\buy-comics-shop-locator.png" alt="digital-comics">
          </div>
          <span>COMIC SHOP LOCATOR</span>        
       </li>
    
       <li>
          <div class="icon-shop">
             <img src="../assets\img\buy-dc-power-visa.svg" alt="POWER VISA">
          </div>
          <span>DC POWER VISA</span>        
       </li>
    
     </ul>
  </div>
</div>
</template>

<script>
export default {
 name: 'ShopSection', 
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';
@import '../assets/style/utilities.scss';

.container-shop{
  height: 120px;
  background-color: $primary-color;
}

.icon-shop{
  width: 40px;
  height: 40px;
  display: inline-block;
  vertical-align: middle;
  margin-right: 8px
}

li span{
  color: white
}


</style>