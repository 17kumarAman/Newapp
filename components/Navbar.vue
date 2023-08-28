<script setup lang="ts">

</script>

<template>
    <div>
        <nav class="bg-cyan-900 ">
            <div class="px-4 max-w-7xl mx-auto sm:px-6 lg:px-8">
                <div class="flex justify-between h-16">
                    <div class="mt-4 sm:ml-6 sm:flex sm:items-center">
                        <NuxtLink to="/" class="text-white px-3 py-2 rounded-md text-sm font-medium hover:bg-cyan-700 focus:outline-none">Home</NuxtLink>
                        <NuxtLink to="/login" class="text-white px-3 py-2 rounded-md text-sm font-medium hover:bg-cyan-700 focus:outline-none">Login</NuxtLink>
                        <NuxtLink to="/registration" class="text-white px-3 py-2 rounded-md text-sm font-medium hover:bg-cyan-700 focus:outline-none">Registration</NuxtLink>
                        <NuxtLink to="/contact" class="text-white px-3 py-2 rounded-md text-sm font-medium hover:bg-cyan-700 focus:outline-none">Contact</NuxtLink>
                        
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>

<style lang="scss" scoped>

</style>