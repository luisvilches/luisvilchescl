<script>
var arr = [
    {
        img:"http://www.cesarcalle.com/images/works/logotipo/17-mademold.jpg",
        title: "Chilito",
        description: "Desarrollo Frontend",
        category: "Frontend"
    },
    {
        img:"http://www.cesarcalle.com/images/works/logotipo/18-ross.jpg",
        title: "Chilito",
        description: "Desarrollo Backends",
        category: "Backends"
    },
    {
        img:"http://www.cesarcalle.com/images/works/logotipo/1-mirapartment.jpg",
        title: "Chilito",
        description: "Desarrollo de la Apps",
        category: "Apps"
    }
];
import ItemsJobs from "./JobsItems"
export default {
name:"four",
data(){
    return {
      items: []
    }
  },
  created(){
      this.cargarJobs();
  },
  methods:{
      cargarJobs: function(){
          this.items = arr;
      },
      filter: function(cat){
        var btns = document.querySelectorAll(".btngroup li button");
        console.log(btns)
        for(var i = 0; i < btns.length; i++){
          if(btns[i] == event.target){
            event.target.classList.add("active");
            console.log("es igual");
          } else {
            btns[i].classList.remove("active");
            console.log("no es igual");
          }
        }
        console.log(event.target)
        if(cat != ""){
          this.items = arr;
          this.items = arr.filter(item => {
            if(item.category.toLowerCase() === cat.toLowerCase()){
              return item;
              }
          });
        } else {
          this.items = arr;
        }
      }
  },
  components:{
    ItemsJobs
  }
}
</script>

<template>
    <div class="main">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <h2 class="text-center">Mis Ultimos Trabajos</h2>
                    <hr>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12 pd">
                    <ul class="btngroup">
                    <li><button type="button" v-on:click="filter('')" class="btn btn-secondary active">Todos</button></li>
                    <li><button type="button" v-on:click="filter('Frontend')" class="btn btn-secondary">Frontend</button></li>
                    <li><button type="button" v-on:click="filter('Backends')" class="btn btn-secondary">Backends</button></li>
                    <li><button type="button" v-on:click="filter('Apps')" class="btn btn-secondary">Apps</button></li>
                    <li><button type="button" v-on:click="filter('Fullstack')" class="btn btn-secondary">FullStack</button></li>
                    </ul>
                </div>
            </div>
            <ItemsJobs :items="items"/>
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

    hr{
        margin-bottom: 45px;
        max-width: 50px;
        border: 1px solid #fff;
    }

    .btngroup{
    text-align: center;
    margin-left: -40px;
  }

  .btngroup li{
    list-style: none;
    display: inline-block;
  }

  .btngroup li button{
    color: #4A57FF;
    background:#fff;
    border: none;
    font-family: 'Comfortaa', cursive;
  } 

  .active{
    background: #4A57FF !important;
    color:#fff !important;
    border: none;
    font-family: 'Comfortaa', cursive;
    border: 1px solid #fff;
  }
</style>
