<script setup >
definePageMeta({
    layout:'custom',
})

const data = await useFetch('https://newsapi.org/v2/everything?q=apple&from=2023-08-27&to=2023-08-27&sortBy=popularity&apiKey=b586ade02a964127a74f707989e024a8')

const articles = computed(()=> data.data.value.articles)


const revenue = ref(123);
    const title = ref('batman')
    const date= ref('11-11-2023')
    const poster = ref('/download.jpeg')
    const overview = ref('Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste tempora odio, eum excepturi error magnam nulla quas deleniti aut minus.')
</script>

<template>
    <div>
        <MovieDetail :title = 'title' :date="date" :poster="poster" :revenue="revenue" :overview="overview"/>
    </div>
</template>
