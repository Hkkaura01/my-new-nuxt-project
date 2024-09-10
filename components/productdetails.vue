<template>
    <div class="card shadow-lg ">
        <div class="grid grid-cols-2">
            <div class="mb-4 mt-4 p-7 border border-r-8  my-4 mx-4">
             <img :src="products.image" class="mx-auto">
            </div>
            <div class="p-7">
                <h4 class="text-4xl truncate my-7 ">{{ products.title }}</h4>
              <h2 class="text-xl font-bold">Price-${{ products.price }}</h2>
              <p class="font-bold border-b-2  mt-4 pb-4 text-center">Products Description</p>
              <p class="text-sm">{{ products.description }}</p>
              <div class="justify-items-center-center items-center">
                <NuxtLink >
            <button class="btn bg-green-500 text-white rounded-sm font-bold p-2 mt-8 items-center ">Add to Cart</button>
        </NuxtLink> 
              </div>
             
              
            </div>
            
        </div>
      
    </div>
      
   
</template>

<script setup>
   const { products}= defineProps(['products'])
</script>
  
<style  scoped>
#body{
    background-color: green;
}
img{
    width: 300px;
    height: 350px;

}
.btn{
    width: 70%;
    height: 40px;
}
</style>