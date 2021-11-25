<template>
<main>
  <div class="jumbo">
     
  </div>
   <div class="fc-container card-container">
      <div class="fc-container button-container-series">
        <button class="button-series">CURRENT SERIES</button>
      </div>
    <ProductCard
     v-for="(product, index) in externalList" :key="index"
     :product="product"   
    />   
  </div>

  <div class="fc-container fc-button">
    <button>LOAD MORE</button>
  </div>
</main>
 
</template>

<script>

import ProductCard from './ProductCard.vue';
import externalList from '../assets/data/productData'
export default {
  name: 'MainSection',
  components: {
    ProductCard
  },

  data(){
    return{
      externalList
    }
  }

}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/utilities.scss';

  main{

    background-color:#1C1C1C;
    color: white;
     .fc-button{
       text-align: center;
       padding: 15px;
        button{
          width: 150px;
          height: 30px;
          border-radius: 0;
          border: none;
          background-color: $primary-color;
          color: white;
          font-weight: bold;
          margin-bottom: 15px;
          cursor: pointer;
          font-size: 12px
        }
     }

     .button-container-series{
       margin-top: -55px
     }

     .button-series{
       padding: 10px;
       background-color: $primary-color;
       color: white;
       border: none;
       font-size: 18px;
       font-weight: bold;
       cursor: pointer;
       
     }
  }

.jumbo{
  width: 100%;
  height: 400px;
  background-image: url('../assets/img/jumbotron.jpg');
  background-size: cover;
}

.card-container{
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding-top: 20px;
  // align-content: flex-start;
  // overflow: hidden;
  padding: 30px;
  cursor: pointer;
}

</style>