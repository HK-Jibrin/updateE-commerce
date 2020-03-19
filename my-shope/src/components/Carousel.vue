<template>
<div class="car">
    
        <carousel :per-page="1" :mouse-drag= "true" :autoplay= true  :loop= true  :speed ="2000">

            <slide v-for="image in carouselImage" :key="image.imageUrl" >
                <img :src="image.imageUrl"  width= 900; height= 500; />
            </slide>
        </carousel>
</div>
    
</template>
<script>

export default {
    name: "jubrin",
    data(){
        return{
            carouselImage:[
          {
         imageUrl: require("../assets/maize.jpg")  
          },
          {
         imageUrl: require("../assets/vegetables.jpg")  
          },
          {
         imageUrl: require("../assets/powerbike.jpg")  
          },
          {
         imageUrl: require("../assets/spinach.jpg")  
          },

        ],
        }
    }
    


}
</script>
<style>

</style>