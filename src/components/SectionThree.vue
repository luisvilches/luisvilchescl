<script>
export default {
  name:"sectionThree"
}
</script>

<template>
    <div class="main">
        <div class="container text-right">
            <div class="row">
                <div class="col-md-8 about">
                    <h2>Sobre Mi</h2>
                    <hr align="right">
                    <p>
                        Soy un joven dedicado a el desarrollo de aplicaciones web y Móviles basadas en los lenguaje de programación mas utilizados del mercado, acompañado de HTML5, JAVASCRIPT y CSS3. Apasionado por los códigos y preparado para afrontar nuevos retos que se presenten a futuro, aprendiendo de los errores para dar soluciones responsables
                    </p>

                    <p class="destacado">
                        ¡Estoy seguro que haremos un buen trabajo juntos!
                    </p>
                </div>
                <div class="col-md-4 pd20">
                    <img class="img-fluid" src="../assets/hacker.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .main{
        background: #fff;
        min-height: 400px;
    }
    h2{
        font-size: 25px;
    }

    .about{
        padding: 80px 40px;
    }

    hr{
        margin-bottom: 80px;
        max-width: 50px;
        border: 1px solid #4A57FF;
    }

    .destacado{
        color:#4A57FF;
    }

    .pd20{
        padding: 100px 40px;
    }

</style>
