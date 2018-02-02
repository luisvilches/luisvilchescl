<template>
  <div class="home">
    <div class="container">
      <div class="row">
        <div class="col-md-6 text-center ">
          <img class="img-fluid img-responsive" src="../assets/tuxedo.png">
        </div>
        <div class="col-md-6">
          <div class="pd40">
            <h5>¡Hola!, soy</h5>
            <h1>Luis Vilches</h1>
          <p class="text-left text1">
            Desarrollador Fullstack y Apps Móviles Freelance
          </p>
          <p>Soy un joven dedicado a el desarrollo de aplicaciones web y Móviles, Apasionado por los códigos y preparado para afrontar nuevos retos que se presenten a futuro</p>
          <button class="btn">¡Saber mas! </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'sectionOne',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style scoped>

  img{
    margin-top: 35px;
    max-width: 450px;
    width   : 100% !important;
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
  h2{
    font-size: 25px;
  }
  .text1{
    font-size: 22px;
  }

  p{
    font-size: 12px;
  }


</style>
