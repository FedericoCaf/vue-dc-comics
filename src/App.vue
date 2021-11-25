<template>
  <div>
   
      <Header/>
   
      <MainSection/>

      <ShopSection/>

      <Footer/>
    
  </div>
</template>

<script>

import Header from './components/Header.vue';
import MainSection from './components/MainSection.vue';
import ShopSection from './components/ShopSection.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
   Header,
   MainSection,
   ShopSection,
   Footer,
  }
}
</script>

<style lang="scss">

  @import "./assets/style/vars.scss";
  @import "./assets/style/generals.scss";
  @import "./assets/style/utilities.scss";

</style>
