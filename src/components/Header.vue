<template>
   <header>
       <div class="fc-container fc-flex-between">
       <div class="logo-header">
         <a href="#">
           <img src="../assets/img/dc-logo.png" alt="logo">
         </a>
       </div>
       <div class="menu-header">
         <nav>
            <ul class="fc-flex-between-align-center">
              <li :class="{'active-border': item.current}" class="fc-flex-align-center" v-for="(item, index) in links" :key="index">
                 <a :class="{'active-text': item.current}" :href="item.url">{{item.text}}</a>
              </li>
            </ul>
        </nav>
       </div>
    </div>
   </header>
  
   
</template>

<script>
export default {
 name: 'Header',

 data(){
   return{
     links:[
        {
          url:'/CHARACTERS',
          text: 'CHARACTERS',
          current: false
        },
        {
          url:'/COMICS',
          text: 'COMICS',
          current: true
        },
        {
          url:'/MOVIES',
          text: 'MOVIES',
          current: false
        },
        {
          url:'/TV',
          text: 'TV',
          current: false
        },
        {
          url:'/GAMES',
          text: 'GAMES',
          current: false
        },
        {
          url:'/COLLECTIBLES',
          text: 'COLLECTIBLES',
          current: false
        },
        {
          url:'/VIDEOS',
          text: 'VIDEOS',
          current: false
        },
        {
          url:'/FANS',
          text: 'FANS',
          current: false
        },
        {
          url:'/NEWS',
          text: 'NEWS',
          current: false
        },
        {
          url:'/SHOP',
          text: 'SHOP',
          current: false
        },
      ]
   }
 }


}

</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/utilities.scss';

 

  .logo-header{
    height: 100px;
    width: 100px;
    padding: 15px;
  }

  .menu-header{
    height: 100px;
    width: 700px;
    font-size: 13px;
    font-weight: bold;
  }

  .active-text{
    color: $primary-color !important;
  }

  .active-border{
    border-bottom: 3px solid $primary-color;
  }

  li{
    height: 100px;
    border-bottom: 3px solid transparent;
     a{
       color: black;
     }
  }


</style>