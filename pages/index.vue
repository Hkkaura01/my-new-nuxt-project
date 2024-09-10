<template>
       <div class="container grid grid-cols-6 flex gap-2 text-center">
        <div v-for="p in product">
     <myproducts :product="p"/>
      
    </div>
       </div>
    
</template>

<script setup>

      const {data:product} = await useFetch('https://fakestoreapi.com/products/')
</script> 

<style scoped>
body{
    margin: 0;
}
</style>
