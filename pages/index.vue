<script setup>
//  Search Movie
    const searchError = ref(false);
    const searchMovie = (searchInput) =>{
        // console.log('Search Text: ', searchInput)
        if(searchInput===''){
            searchError.value=true;
        }if(searchInput !== ''){
            searchError.value=false
        }
    }

    // Fetch Movie
    const data = await useFetch('https://newsapi.org/v2/everything?q=apple&from=2023-08-27&to=2023-08-27&sortBy=popularity&apiKey=b586ade02a964127a74f707989e024a8')
    // console.log(data.data.value.articles)
    // const movieid = ref(123);
    // const title = ref('batman')
    // const date= ref('11-11-2023')
    // const poster = ref('/download.jpeg')


const articles = computed(()=> data.data.value.articles)
// console.log(articles);
</script>

<template>
    <div>
        <searchBar @search-movie="searchMovie" :searchError="searchError"/>
        <div class="grid md:grid-cols-4 sm:grid-cols-1 justify-items-center bg-cyan-50 ">
            <div v-for="news in articles">

                <MovieCard :title = 'news.title' :date="news.publishedAt" :poster="news.urlToImage" :url="news.url" :description="news.description" />
                <!-- {{ news }} -->
            </div>
            
        </div>
    </div>
</template>

