<template>
  <div  >
    <div class="row mt-md-5 mt-sm-5 mt-xs-5">
      <div
        class="col-lg-6 col-xs-12"
        v-for="(movie, index) of movies"
        :key="index"
      >
        <div class="d-flex justify-content-left align-items-start bg-dark text-white rounded m-3" style="height: 250px;">
          <div class="p-3">
            <img :src="movie.Poster" alt="movie poster" class="rounded"/>
          </div>

          <div class="p-2 col">
            <h2>{{ movie.Title}}</h2>
            <br>
            <p><span><b>Tipo: </b> </span>{{ movie.Type }}
            <br>
            
            <span><b>Año: </b> </span>{{ movie.Year }}</p>
            <br>
            <br>
            
          <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
          <a
            :href="'https://www.imdb.com/title/' + movie.imdbID"
            class="btn btn-light " target="_blank"
            >Info</a>
        </div>
          </div>
        </div>
        
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "SectionApi",
  data() {
    return {
      movies: null,
    };
  },
  mounted() {
    axios
      .get("http://www.omdbapi.com/?s=spider+man&type=movie&apikey=25d49bb1")
      .then((response) => {
        this.movies = response.data.Search.slice(0, 4);
        
      });
  },
};
</script>

<style scoped>

img{
  max-width: 150px;
};
</style>