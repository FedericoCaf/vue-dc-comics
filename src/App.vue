<template>
  <div>
     <Header/>
    <main>MAIN</main>
    <section>SECTION</section>
    <footer>FOOTER</footer>
  </div>
</template>

<script>

import Header from './components/Header.vue';


export default {
  name: 'App',
  components: {
   Header,
  }
}
</script>

<style lang="scss">

  @import "./assets/style/vars.scss";
  @import "./assets/style/generals.scss";
  @import "./assets/style/utilities.scss";

</style>
