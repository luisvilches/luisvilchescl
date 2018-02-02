<script>
export default {
  name: "sectionFive",
  data () {
    return {
      
    }
  },
  methods:{
    enviar: function(){
      console.log(document.formulario)
      alert("enviado")
    }
  }
}
</script>

<template>
    <div class="main">
        <div class="container">
            <div class="row">
                <div class="col-md-12 text-center servicios">
                    <h2>¿Tienes un proyecto en mente?</h2>
                    <h6>¡Contactame!</h6>
                    <hr>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12">
                    <form id="myForm" action="mail.php" method="post" class="contact-form">
                        <div class="row justify-content-center">
                            <div class="col-lg-5">
                                <input name="fname" placeholder="Ingresa tu Nombre" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Ingresa tu Nombre'" class="common-input mt-20" required="" type="text">
                            </div>
                            <div class="col-lg-5">
                                <input name="email" placeholder="Ingresa tu Correo" pattern="[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{1,63}$" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Ingresa tu Correo'" class="common-input mt-20" required="" type="email">
                            </div>
                            <div class="col-lg-10">
                                <textarea class="common-textarea mt-20" name="message" placeholder="Ingresa tu Mensaje" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Ingresa tu Mensaje'" required=""></textarea>
                        </div>
                        <div class="col-lg-10 d-flex justify-content-end">
                            <button class="primary-btn white-bg d-inline-flex align-items-center mt-20"><span class="mr-10">Enviar</span><span class="lnr lnr-arrow-right"></span></button> <br>
                        </div>
                        <div class="alert-msg"></div>
                        </div>
                    </form>
                </div>
            </div>
            <!--div class="row">
                <div class="col-md-3">
                    <ul>
                        <li><i class="fa fa-whatsapp"></i></li>
                        <li>+56 9 8492 3552</li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <ul>
                        <li><i class="fa fa-facebook"></i></li>
                        <li>@lvilches21</li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <ul>
                        <li><i class="fa fa-linkedin"></i></li>
                        <li>Luis Vilches</li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <ul>
                        <li><i class="fa fa-envelope-square"></i></li>
                        <li>hola@luisvilches.cl</li>
                    </ul>
                </div>
            </div-->
        </div>
    </div>
</template>

<style scoped>
    .main{
        background: #4A57FF;
        color: #fff;
        min-height: 300px;
        padding: 40px;
    }

    ul{
        background: #fff;
        border-radius: 15px;
        text-align: center;
        padding: 10px;
    }

    ul li{
        list-style: none;
        display: inline-block;
        color: #4A57FF;
    }


    h2{
        font-size: 25px;
    }

    .servicios hr{
        margin-bottom: 80px;
        max-width: 50px;
        border: 1px solid #fff;
    }

    .service-box i{
        color:#fff!important;
        font-size: 40px;
        margin-bottom: 20px;
    }
    .service-box h3{
        font-size: 20px;
    }
    .service-box p{
        font-size: 12px;
        color:#ccc!important;
    }

    .campo{
        margin-bottom: 10px;
    }

    .campo label{
        font-size: 12px;
        font-family: 'Comfortaa', cursive;
    }

    .campo form{
        max-width: 400px;
    }

    .campo input,.campo textarea{
        border-radius: 50px;
    }

    .common-input {
        border: 1px solid #fff;
        line-height: 48px;
        width: 100%;
        display: block;
        background: transparent;
        padding: 0 25px;
        color: #fff;
    }

    .common-textarea {
        border: 1px solid #fff;
        width: 100%;
        display: block;
        background: transparent;
        padding: 15px 25px;
        color: #fff;
        height: 150px;
        resize: none;
    }

    .mt-20 {
        margin-top: 20px;
    }

    ::placeholder { color: white; }
    :-ms-input-placeholder { color: white; } /* IE 10+ */
    ::-webkit-input-placeholder { color: white; } /* WebKit */
    ::-moz-placeholder { color: white; } /* Firefox 19+ */

    .primary-btn.white-bg {
        background: #fff;
        border: 1px solid #eee;
        color: #4A57FF;
    }

    .primary-btn {
        line-height: 40px;
        padding: 0 30px;
        border-radius: 20px;
        background: transparent;
        border: 1px solid #fff;
        color: #222;
        display: inline-block;
        font-weight: 500;
        position: relative;
        -webkit-transition: all 0.3s ease 0s;
        -moz-transition: all 0.3s ease 0s;
        -o-transition: all 0.3s ease 0s;
        transition: all 0.3s ease 0s;
        cursor: pointer;
        text-transform: uppercase;
    }

    form {
        margin-bottom: 40px;
    }
</style>
