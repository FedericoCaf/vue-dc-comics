<template>
  <footer>
  
       <div class="footer-top">
         <div class="fc-container fc-flex-between">
           <div class="footer-list-left">
             <div class="footer-list">
                <ul>
                  <li> <strong> DC COMICS </strong> </li>
                  <li>Characters</li>
                  <li>Comics</li>
                  <li>Movies</li>
                  <li>Games</li>
                  <li>videos</li>
                  <li>News</li>
                </ul>
                <ul>
                  <li> <strong> SHOP </strong> </li>
                  <li>Shop DC</li>
                  <li>Shop DC collectibles</li>
                </ul>
            </div>
            <div class="footer-list">
                <ul>
                  <li> <strong> DC </strong> </li>
                  <li>Terms of use</li>
                  <li>Privacy policy(new)</li>
                  <li>Ad Choices</li>
                  <li>Advertising</li>
                  <li>Jobs</li>
                  <li>Subscription</li>
                  <li>Talent Workshops</li>
                  <li>CPSC Certificates</li>
                  <li>Ratings</li>
                  <li>Shop Help</li>
                  <li>Contact Us</li>
                </ul>
            
            </div>
            <div class="footer-list">
                <ul>
                  <li> <strong> SITES </strong> </li>
                  <li>DC</li>
                  <li>MAD magazine</li>
                  <li>DC kids</li>
                  <li>DC universe</li>
                  <li>DC power visa</li>
                </ul>
            </div>
       
          </div>

          <div class="footer-img-right">
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
         </div>
          
    </div>
   
   

   <div class="footer-bottom fc-flex-between-align-center">
     <div class="fc-container fc-flex-between-align-center">
       <div class="sign-up">
         <button>SIGN UP NOW!</button>
       </div>
       <div class="social fc-flex-between-align-center">
         <span>FOLLOW US</span>
         <div class="social-icon">
           <img src="../assets/img/footer-facebook.png" alt="facebook">
         </div>
         <div class="social-icon">
           <img src="../assets/img/footer-twitter.png" alt="twitter">
         </div>
         <div class="social-icon">
           <img src="../assets/img/footer-youtube.png" alt="youtube">
         </div>
         <div class="social-icon">
           <img src="../assets/img/footer-pinterest.png" alt="pinterest">
         </div>
         <div class="social-icon">
           <img src="../assets/img/footer-periscope.png" alt="periscope">
         </div>
       </div>
    </div>
   </div>
    
      
</footer>
</template>

<script>
export default {
 name: 'Footer',
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/utilities.scss';

footer{

   .footer-top{
     background-image:url("../assets/img/footer-bg.jpg");
     background-position: center;
     background-size: cover;
     height: 300px;
     overflow: hidden;
  
   }
   .footer-bottom{
     height: 80px;
     background-color: #303030;
   }
}

ul{
  padding-top: 25px;
   li{
     margin: 5px;
   }
}

ul li:first-child{
  padding-bottom: 10px;
  color: white;
}

.footer-list{
  display: inline-block;
  padding-right: 20px;
  color:#7C7C7C;
  font-size: 13px;
  overflow: hidden;
}

.sign-up button{
  padding: 12px;
  border: 2px solid $primary-color;
  background-color: #303030;
  color: white;
   cursor: pointer;
}

.social{
  color: white;
   .social-icon{
     padding-left: 10px;
     cursor: pointer;
   }
}

.footer-img-right{
  position: relative;
  width: 560px;
  // height: 560px;
}

.footer-img-right img{
  position: absolute;
  top: -140px;
  right: 0;
}



</style>