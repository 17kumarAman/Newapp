<script setup lang="ts">

    function Submit(){
        alert('Okay We will contact u.')
        
    }
</script>

<template>
    <div class="flex flex-col md:flex-row">
        <div class="md:w1/2 p-8">
            <img src="https://cdn.pixabay.com/photo/2015/11/03/08/58/meeting-1019875_960_720.jpg" alt="Contact US">
        </div>
        <div class="md:w-1/2 p-8 shadow-md">
            <p class="text-lg mb-2">
                123 Main Street <br> Ranchi, India 12345
            </p>
            <p class="text-lg mb-2">
                Phone: (123) 456-7890 <br> Email: info@1234code.com
            </p>
            <form action="">
                <label for="name" class="block text-lg font-bold mb-2" >Name</label>
                <input type="text" id="name" name="name" class="w-full border border-gray-300 p-2 mb-4 rounded-lg" />
                <label for="email" class="block text-lg font-bold mb-2" >Email</label>
                <input type="text" id="email" name="email" class="w-full border border-gray-300 p-2 mb-4 rounded-lg">
                <label for="message" class="block text-lg font-bold mb-2" >Message</label>
                <textarea  id="message" name="message" class="w-full border border-gray-300 p-2 mb-4 rounded-lg"></textarea>
                <!-- <h1 class="bg-black text-white text-3xl">{{ name }}</h1> -->
                <button class="bg-rose-500 hover:bg-rose-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline " @click="Submit" type="submit">Submit</button>
            </form>
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>