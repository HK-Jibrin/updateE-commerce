<template>
<div class="hom">
   <div class="products">
           <img :src="product.imageLink" height="150" width="250">
    <p>{{product.name}}  </p>
    <p> &#8358; {{product.price}} </p>
    <b-button href="#" variant="primary" style="margin-bottom: 10px;"> Buy Now </b-button>  
   </div>
</div>
      
</template>
<script>

export default {
    name: 'Products',
    props: ["product"]
}
</script>
<style scoped>
.products{
    padding: 0;
    margin: 0;
    margin-left: 10px;
    margin-bottom: 10px;
    border: 2px solid black;
    text-align: center;
    padding-top: 20px;
    background-color: whitesmoke;
    border-radius: 20px;
}
.hom{
  width: 300px; 
  margin-bottom: 10px;
  
   display: inline-block;
}
 

</style>










