<script>
export default {
  name: "sectionTwo"
}
</script>

<template>
    <div class="main" id="about">
        <div class="container">
            <div class="row">
                <div class="col-md-12 text-center servicios">
                    <h2>Mis Servicios</h2>
                    <hr>
                </div>
            </div>
            <div class="row">
                <div class="col-lg-3 col-md-3 text-center">
                    <div class="service-box">
                        <i class="material-icons text-primary sr-icons">lightbulb_outline</i>
                        <h3>Fábrica de Ideas</h3>
                        <p class="text-muted">Juntos crearemos una gran propuesta, que se adapte a tu negocio y tus necesidades.</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-3 text-center">
                    <div class="service-box">
                        <i class="material-icons text-primary sr-icons">desktop_windows</i>
                        <h3>Responsive Design</h3>
                        <p class="text-muted">Diseños interactivos, atractivos y amigables. Adaptables a todo tipo de dispositivo.</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-3 text-center">
                    <div class="service-box">
                        <i class="material-icons text-primary sr-icons">apps</i>
                        <h3>Aplicaciones</h3>
                        <p class="text-muted">Desarrollo de aplicaciones nativas e híbridas, nos ajustamos a los requerimientos de tu idea de negocio.</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-3 text-center">
                    <div class="service-box">
                        <i class="material-icons text-primary sr-icons">build</i>
                        <h3>Asistencia Técnica</h3>
                        <p class="text-muted">Cambios y reestructura de sitios o aplicaciones ya implementados, asistencia técnica a todos nuestros desarrollos.</p>
                    </div>
                </div>
            </div>
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
</style>
