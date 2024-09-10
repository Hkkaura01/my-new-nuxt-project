<template>
         <div>
            <Productdetails :products="products" />
         </div>
         
</template>

<script setup>
   const {id}=useRoute().params
   const api = 'https://fakestoreapi.com/products/'+ id;
   const {data:products}=await useFetch(api)
</script>

<style scoped>
  img{
    width: 189px;
    height: 300px;
  }
</style>



