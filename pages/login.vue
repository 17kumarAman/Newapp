<script setup >
    definePageMeta({
        layout:'custom'
    });
    function Submit(){
        setTimeout(() => {
            alert('Welcome Back')
        }, 500);
        
        
    }
</script>
<template>
    <div class="w-full max-w-md mx-auto mt-5">
        <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4">
            <div class="mb-4">
                <label for="username" class="block text-gray-700 font-bold mb-2">Username</label>
                <input type="text" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="username" placeholder="Username">
            </div>
            <div class="mb-4">
                <label for="username" class="block text-gray-700 font-bold mb-2">Password</label>
                <input type="password" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="password" placeholder="Passwors">
            </div>
            <div class="flex items-center justify-center mt-6">
                <NuxtLink href="/"><button @click="Submit" class="bg-rose-500 hover:bg-rose-700 text-white font-bold py-2 px-8 rounded-full focus:outline-none focus:shadow-outline " type="submit">Login</button></NuxtLink>
                
            </div>
        </form>
    </div>
</template>