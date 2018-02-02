<script>

  import Navbar from "./components/Navbar"
  import Footer from "./components/Footer"
  export default {
    name: 'app',
    data () {
      return {
        title: 'luisvilches2'
      }
    },
    components:{
      Navbar,
      Footer
    }
  }
</script>


<template>
  <div id="app">
    <div class="boxshadow">
      <Navbar />
      <router-view></router-view>
      <Footer />
    </div>
  </div>
</template>

<style>
  #app{
    padding: 40px;
  }

  body{
    background: #f6f6fc;
    font-family: 'Comfortaa', cursive;
  }
  .boxshadow{
    box-shadow: 0px 0px 50px 0px rgba(0,0,0,0.2);
  }
</style>
