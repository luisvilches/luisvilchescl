<script>
export default {
  name: "itemsJobs",
  props: ["items"]
}
</script>


<template>
    <div class="row top">
        <div class="col-md-4 " v-for="(item,index) in items" :key="index">
            <div class="card text-center">
                <img class="img-fluid" :src="item.img" :alt="item.title">
                
            </div>
            
        </div>
    </div>
</template>

<style scoped>
    img{
        width: 100%;
        border-radius: 15px;
    }

    .top{
        margin-top: 20px;
    }

    h4,p{
        font-family: 'Comfortaa', cursive;
    }

    .card{
        margin-bottom: 40px;
        border-radius: 15px;
    }
    
    .card:hover {
        -webkit-box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
                box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        -webkit-transition: all ease .1s;
        transition: all ease .1s;
    }

</style>
