<script setup lang="ts">
    const props = defineProps(['newsid', 'title', 'date','poster','url','description'])
    // console.log(props)
</script>

<template>
    <div class="bg-cyan-5500 roounded-lg shadow-md overflow-hidden m-4 px-2 ">
        <div class="p-1 py-4 ">
            <h3 class="font-semibold text-lg mb-2 text-center">{{title.length<50?title+'...':title.slice(0,50)+'...'}}</h3>
            <div class="overflow-hidden mb-4">
                <img :src="poster" alt="Placeholder Image" class="h-200 w-300 object-cover"/>
            </div>
            <p class="text-black text-bold text-sm mb-2 px-2">{{description.length<150?description:description.slice(0,150)+'...'}}</p>
            <p class="text-gray-500 text-sm mb-2 px-2">Release Date: {{date}}</p>
            <div class="mt-4 p-2 text-right">
                <!-- <NuxtLink :to="`${url}`" class="bg-rose-500 hover:bg-rose-600 text-white font-medium py-2 px-4 rounded ">Get Details</NuxtLink> -->
                <a :href= 'url' class="bg-rose-500 hover:bg-rose-600 text-white font-medium py-2 px-4 rounded ">Get Details</a>
            </div>
        </div>
    </div>
</template>

<style scoped>
.h-400{
    height:400px;
}
.w-300{
    width: 300px;
}
</style>