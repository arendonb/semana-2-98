<template>
    <div id="app">

  <div class="container-fluid">
  <div class="row justify-content-center mb-5" >
    <div class="col mt-5" v-for="(item, index) of team" :key="index">
    <team-card v-bind:member="item"></team-card>
    </div>
  </div>
  </div>

    <page-footer></page-footer>
    <h1>{{title}}</h1>
  </div>
</template>

<script>

import PageFooter from './components/PageFooter.vue'
import TeamCard from './components/TeamCard.vue'



export default {
  name: 'App',
  components:{
    PageFooter,
    TeamCard,

  },
  data(){
    return{
      title:'Vivo dentro de VUE',
      team: [
        {
          codigo: 1,
          nombre: "Santiago Andrés Millan Pardo",
          descripcion: 'Estudiante de Ingenieria de Telecomunicaciones en la Universidad Santo Tomas. Apacionado por el deporte,desarrollo de herramientas tecnologias y la gestion de procesos. Amor por las dos ruedas.',
          rol: "Desarrollador Backend",
          imagen: 'https://placeimg.com/192/192/people',
        },
        {
          codigo: 2,
          nombre: "Cristhian Daniel Diaz Salazar",
          descripcion: 'Ingeniero Industrial de la Universidad Tecnológica de Pereira. Me dedico a administrar hoteles en Pereira. Apasionado por la ciencia, la tecnología y los sistemas de información. Mi pasatiempo favorito es jugar videojuegos.',
          rol: "Scrum Master",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 3,
          nombre: "Miguel Enrique Marquez Aldana",
          descripcion: 'Supervisor de prospección geofísica con más de 16 años de experiencia en la planeación, supervisión y ejecución de registro de ondas sísmicas, con habilidad para el trabajo en diferentes tipos de terreno y en un ambiente multicultural.',
          rol: "Tester",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 4,
          nombre: "Diego Luis Soto Mendoza",
          descripcion: '4.Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.',
          rol: "FrontEnd",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 5,
          nombre: "Alejandro Rendón Blandón",
          descripcion: 'Ingeniero electrónico, especialista en Telecomunicaciones, especialista en Gerencia de Proyectos de la Universidad Pontificia Bolivariana en Medellín. Mi pasatiempo favorito es viajar en moto por todo el mundo, compartiendo con mis amigos.',
          rol: "Product Owner",
          imagen: "https://placeimg.com/192/192/people",
        }
      ]
    }
  }
}
</script>

