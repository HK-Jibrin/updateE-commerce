<template>
  <div class="home">
    <Header />
<b-container class="bv-example-row" fluid>
  
  <b-row>
    <b-col cols><category v-for="cat in categories" :key="cat.id" :category="cat"/></b-col>
    <b-col cols ="9"><div id="cal"><Carousel /></div></b-col>
    
    
  </b-row>
</b-container>
      <div class="down"><Products v-for="item in products" :key="item.id" :product="item" /></div>
      <div>
        <Footer/>
      </div>
</div>

</template>

<script>
// @ is an alias to /src
import Category from '../components/Category.vue'
import Header from '../components/Header.vue'
import Products from '../components/Products.vue'
import Carousel from '../components/Carousel.vue'
import Footer from  '../components/Footer.vue'

export default {
  name: 'Home',
 components :{
    Category, 
    Header,
    Products,
    Carousel,
    Footer
   
  },
  data(){
      return{

        categories: [
          {
            id : 1,
        name: 'Female Shoes',
        
          
        },
        {
            id : 2,
        name: "Men's Wear  ",
        
        },
        {
            id : 3,
        name: 'Laptops',
        
          
        },
    {
            id : 4,
        name: 'Bags',
        
          
        },
        {
            id : 5,
        name: "vegetables",
        
           },
            {
            id : 6,
        name: "Cars",
            }
        ],

    products: [
        {
        id: 1,
        imageLink: require("../assets/f3shoe.jpg") ,
        name: 'Female Shoe',
        price: 35000
        },
         {
         id: 2,
         imageLink: require("../assets/f2shoe.jpg") ,
        name: 'Female Shoe2',
        price: 40000
         },
        {
        id: 3,
        imageLink: require("../assets/shortsleave.jpg") ,
        name: 'Male Shirt',
        price: 20000
        },
        {
        id: 4,
        imageLink: require("../assets/images.jpg") ,
        name: 'Laptop',
        price: 120000
        },
        {
        id: 6,
        imageLink: require("../assets/g4.jpg") ,
        name: 'Bag',
        price: 5000
        },
        {
        id: 7,
        imageLink: require("../assets/malewear.jpg") ,
        name: 'Male Shirt',
        price: 4000
        },
        {
        id: 8,
        imageLink: require("../assets/yam-1.jpg") ,
        name: 'Tuber of Yam',
        price: 700
        },
        {
        id: 9,
        imageLink: require("../assets/spinach.jpg") ,
        name: 'Natural Spinach',
        price: 500  
        },
         {
        id: 10,
        imageLink: require("../assets/benz.jpg"),
        name: 'Mercedees benz c300',
        price: 75.7 
        },{
        id: 11,
        imageLink: require("../assets/suzukibrezza.jpg") ,
        name: 'Suzuki Brezza',
        price: 25.9
        },
    ]

    }
  }

  }
</script>

<style>

.down{
  margin-top: 40px;
}
.bv-example-row{
 margin-top: 10px;
}

</style>
