<template>
<div id="app">
  <div class="container-fluid">
   
        <section-api> </section-api>
      </div>



    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <team-card></team-card>
      </div>
    </div>

    <page-footer></page-footer>
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
import PageFooter from "./components/PageFooter.vue";
import TeamCard from "./components/TeamCard.vue";
import SectionApi from "./components/SectionApi.vue";

export default {
  name: "App",
  components: {
    PageFooter,
    TeamCard,
    SectionApi,
  },
  data() {
    return {
      title: "Vivo dentro de VUE",
      team: [
        {
          codigo: 1,
          nombre: "Primer Integrante",
          descripcion:
            "1.Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
          rol: "desarrollador Backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 2,
          nombre: "Segundo Integrante",
          descripcion:
            "2.Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
          rol: "desarrollador Backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 3,
          nombre: "Tercer Integrante",
          descripcion:
            "3.Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
          rol: "desarrollador Backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 4,
          nombre: "Cuarto Integrante",
          descripcion:
            "4.Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
          rol: "desarrollador Backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 5,
          nombre: "Quinto Integrante",
          descripcion:
            "5.Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.",
          rol: "desarrollador Backend",
          imagen: "https://placeimg.com/192/192/people",
        },
      ],
    };
  },
};
</script>

