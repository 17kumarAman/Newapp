<script setup lang="ts">
    defineProps(['revenue', 'overview', 'title', 'date','poster'])


</script>

<template>
    <div class="grid sm:grid-cols-3 gap-7 justify-items-center m-10">
        <div class="bg-white rounded-lg shadow-md overflow-hidden">
            <img :src="poster" alt="Placeholder Image" class="h-400 w-full object-cover" />
        </div>
        <div class="sm:col-span-2 mx-6">
            <h1 class="font-bold text-2xl mb-5">{{title}}</h1>
            <h3 class="font-semibold text-lg mb-5">Release Date: {{date}}</h3>
            <p class="text-gray-500 text-md mb-8">{{overview}}</p>
            <p class="text-gray-500 text-md">Revenue: $ {{revenue}}</p>
            <div class="mt-6">
                <NuxtLink to="https://www.youtube.com/watch?v=LIkIVD9apl4" target="_blank" class="bg-indigo-500 hover:bg-indigo-600 text-white font-medium py-2 px-4 rounded ">Watch Trailer</NuxtLink>
                <button  class="bg-rose-500 hover:bg-rose-600 text-white font-medium py-2 px-4 rounded m-5">Buy Now</button>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>