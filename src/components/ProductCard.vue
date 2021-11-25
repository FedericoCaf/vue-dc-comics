<template>

  <div class="product-card">
       <img :src="product.thumb" :alt="product.series">
      <span> {{product.series}} </span>
  </div>
    
</template>

<script>
export default {
 name: 'ProductCard',
 props: {
   product: Object,
 }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/utilities.scss';

.product-card{
  // position: relative;
  flex-basis: calc((100% / 6) - 20px);
  height: 175px;
  margin: 20px 10px 100px 10px;
}

.product-card img{
  width: 100%;
}

@media (max-width:1170px) {
  .product-card{
    flex-basis: calc((100% / 4) - 40px);
  }
  
}
@media (max-width:992px) {
  .product-card{
    flex-basis: calc((100% / 2) - 200px);
    height: 350px;
    margin-right: 200px;
  }
  
}

</style>