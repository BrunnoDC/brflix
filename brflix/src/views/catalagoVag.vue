<script>
  import axios from "axios ";
import CardComp from "../components/CardComp.vue";
export default {
  components: { CardComp },
  data() {
    return {
      generos: [],
      filmesPorGenero: [],
      movies: [
        {
          id: 1,
        },
        {
          id: 2,
        },
        {
          id: 3,
        },
        {
          id: 4,
        },
        {
          id: 5,
        },
        {
          id: 6,
        },
      ],
    };
  },
  async created() {
    const { data } = await axios.get(
      "https://api.themoviedb.org/3/genre/movie/list?api_key=cdd74c9f441352e6a6aee5e2cc6532e6&language=pt-br"
    );
    for (const genero of data.genres) {
      const { data } = await axios.get(
        `https://api.themoviedb.org/3/discover/movie?api_key=cdd74c9f441352e6a6aee5e2cc6532e6&language=pt-BR&sort_by=popularity.desc&include_adult=false&include_video=false&page=1&with_genres=${genero.id}&with_watch_monetization_types=flatrate`
      );
      this.filmesPorGenero.push({
        id: genero.id,
        name: genero.name,
        movies: data.results,
      });
    }
    console.log(this.filmesPorGenero);
    this.generos = data.genres;
  },
  methods: {
    async getMoviesByGenre(genre) {
      const { data } = await axios.get(
        `https://api.themoviedb.org/3/discover/movie?api_key=cdd74c9f441352e6a6aee5e2cc6532e6&language=pt-BR&sort_by=popularity.desc&include_adult=false&include_video=false&page=1&with_genres=${genre}&with_watch_monetization_types=flatrate`
      );
      return data.results;
    },
  },
};
</script>

<template>
    <div class="main">
        <div class="lista">
            <h2 class="txtprin">Mais Procurados</h2>
            <hr>
            <div class="categorias">
                <span>ação</span>
                <span>Comedia</span>
                <span>Drama</span>
            </div>
        </div>
    </div>
</template>
<style>
.bemvindo {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 35%;
  color: white;
  font-size: 1.8rem;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: bold;
  background-color: black;
}

.bemvindo button {
  padding: 15px;
  border-radius: 25px;
  text-decoration: none;
  border: none;
  min-width: 140px;
  cursor: pointer;
  background-color: #1db954;
  margin-top: 15px;
}
.btnenter a {
  color: black;
}
</style>
