<template>
    <div class="card shadow-md p-7 bg-white rounded-lg">
        <div class="justify-center items-center p-5"> 
            <img :src="product.image" class="flex h-auto max-w-full ">
            <h2 class="text-bold truncate">{{ product.title }}</h2>
            <h2 class="font-bold">Price-${{ product.price }}</h2>
        </div>
        <NuxtLink :to="`${product.id}`">
            <button class="btn bg-green-500 text-white rounded-sm font-bold p-2 flex">View Details</button>
        </NuxtLink> 
                    

    </div>

   

</template>


<script setup>
     const {product}=defineProps(['product'])
</script>

<style  scoped>
.cward{
    max-width: 80%;
    max-height: 120px;
    
}
img{
    width: 100px;
    height: 150px;
}
</style>