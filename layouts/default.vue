<template>
    <div class="conatiner">
         <header class="shadow-sm p-4 mx-auto">
            <nav class="flex mx-auto justify-between ">
                <NuxtLink class="nuxt font-bold">MY NUXT-PROJECT</NuxtLink>
                <ul class="flex justify-between gap-4">
                    <li>
                        <NuxtLink to="/">HOME</NuxtLink>
                    </li>

                    <li>
                        <NuxtLink to="/Store/appsite.vue">APP SITE</NuxtLink>
                    </li>

                    <li>
                        <NuxtLink to="/Store/about">ABOUT</NuxtLink>
                    </li>

                    <li>
                        <NuxtLink to="/Store/item" class="btn px-4 py-2 text-white rounded-lg">ITEM</NuxtLink>
                    </li>
                </ul>
            </nav>
         </header>
    </div>
    <div class="container mt-5 justify-center mx-auto">
   <slot />
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style  scoped>
.nuxt{
    color:blue;
    font-size: larger;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
.btn{
    background-color: rgb(20, 127, 248);

}
</style>