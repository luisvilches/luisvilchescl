<script>
export default {
  name:"Navbar",

  methods:{

  }
}
</script>

<template>
    <nav class="navbar navbar-fixed-top navbar-toggleable-md navbar-inverse bg-inverse">
        <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="material-icons">menu</span>
        </button>
        <a class="navbar-brand" href="/"><i class="material-icons">code</i></a>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto"></ul>
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link" href="https://m.me/lvilches21"><i class="fab fa-facebook-messenger"></i></a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="https://api.whatsapp.com/send?phone=56984923552"><i class="fab fa-whatsapp"></i></a></a>
            </li>
          </ul>
        </div>
      </nav>
</template>

<style scoped>
    .bg-inverse{
        background: #fff !important;
    }

    .navbar-inverse .navbar-nav .nav-link{
        color: #000;
    }

    .navbar-inverse .navbar-brand, .navbar-inverse .navbar-toggler{
        color:#000;
    }
</style>
