<template>
  <div class="home">
    <SectionOne/>
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <Maps />
    <SectionFive />
  </div>
</template>

<script>

import SectionOne from "./SectionOne"
import SectionTwo from "./SectionTwo"
import SectionThree from "./SectionThree"
import SectionFour from "./SectionFour"
import SectionFive from "./SectionFive"
import Maps from "./Map"
export default {
  name: 'home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    Maps
  }
}
</script>

<style scoped>

  img{
    margin-top: 35px;
    max-width: 450px;;
  }
  .home{
    background: #fff;
    min-height: 600px;
  }

  button{
    background: #4A57FF;
    color: #fff;
    border-radius: 50px;
    padding: 10px 60px;
    margin-top: 30px;
  }

  .pd40{
    padding: 130px 40px 80px ;
  }

  h1{
    font-size: 60px;
  }
  .text1{
    font-size: 22px;
  }

  p{
    font-size: 12px;
  }


</style>
