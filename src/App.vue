<template>
  <div id="app">
    <MovieCard v-for="(movie, index) in movies" :key="index" :title="movie.title" :image="movie.image" />
  </div>
</template>

<script>
import MovieCard from "./components/MovieCard.vue";

export default {
  name: 'App',
  data(){
    return{
      movies: [
        {title: 'El señor de los anillos', image: 'https://es.web.img3.acsta.net/medias/nmedia/18/89/67/45/20061512.jpg'},
        {title: 'Interestelar', image: 'https://images-na.ssl-images-amazon.com/images/S/pv-target-images/79194981293eabf6620ece96eb5a9c1fffa04d3374ae12986e0748800b37b9cf._RI_TTW_.jpg'},
        {title: 'Avatar', image: 'https://images-na.ssl-images-amazon.com/images/S/pv-target-images/ae4816cade1a5b7f29787d0b89610132c72c7747041481c6619b9cc3302c0101._RI_TTW_.jpg'},
        {title: 'Gladiador', image: 'https://es.web.img3.acsta.net/medias/nmedia/18/70/92/02/20149073.jpg'}
      ]
    }      
  }, 
  components: {
    MovieCard   
  }  
};
</script>

