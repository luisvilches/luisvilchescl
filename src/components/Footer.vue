<script>
export default {
  name: "footer"
}
</script>

<template>
  <div class="main">
      <div class="container">
          <div class="row pd  text-center">
              <div class="col-md-12">
                  <ul>
                      <li><a href="https://api.whatsapp.com/send?phone=56984923552"><i class="fab fa-whatsapp"></i></a></li>
                      <li><a href="https://m.me/lvilches21"><i class="fab fa-facebook-messenger"></i></a></li>
                      <li><a href="https://www.facebook.com/lvilches21"><i class="fab fa-facebook"></i></a></li>
                      <li><a href="https://www.linkedin.com/in/lvilches21/"><i class="fab fa-linkedin"></i></a></li>
                      <li><a href="mailto:hola@luisvilches.cl"><i class="fa fa-envelope-square"></i></a></li>
                  </ul>
              </div>
              <div class="col-md-12">
                  <h6>Luis Vilches  ©  2018 - Todos los derechos reservados. - Hecho con <i class="fas fa-heart"></i></h6>
              </div>
          </div>
      </div>
  </div>
</template>

<style scoped>
    .pd{
        padding: 20px;
    }
    ul{
        margin:40px;
    }

    ul li{
        display: inline-block;
        list-style: none;
    }

    ul li a{
        color: #fff;
         background: #c8d6e5;
        padding: 18px 20px;
        border-radius: 50px;
    }

    ul li a:hover{
        color: #4A57FF;
        background: #fff;
        
    }

    .fa-heart{
        color:#4A57FF;
    }
</style>
