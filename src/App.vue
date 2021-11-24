<template>
  <div>
     <header>
        <Header/>
     </header>
   
      <MainSection/>

      <ShopSection/>
    
    
    <footer>FOOTER</footer>
  </div>
</template>

<script>

import Header from './components/Header.vue';
import MainSection from './components/MainSection.vue';
import ShopSection from './components/ShopSection.vue';


export default {
  name: 'App',
  components: {
   Header,
   MainSection,
   ShopSection,
  }
}
</script>

<style lang="scss">

  @import "./assets/style/vars.scss";
  @import "./assets/style/generals.scss";
  @import "./assets/style/utilities.scss";

  header{
    height: 100px;
  }

   main{
    height: 100px;
    width: 100%;
    background-color: black;
    color: white;
  }


</style>
