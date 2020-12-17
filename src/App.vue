<template>
  <div id="app">

    <!-- Image and text -->
    <imageText></imageText>

    <!-- carousel -->
    
    <carousel></carousel>

    <!-- services -->
    <services></services>

    <!-- news -->
    <div class="container-fluid" id="Newsnave">
      <newsSection></newsSection>
    </div>

    <!-- members -->
    <div class="container-fluid" id="Teamnave">
      <div class="row justify-content-center mb-5">
        <div class="col mt-5 d-flex" v-for="(miembro, index) of Team" :key="index">
          <teamCard :member=miembro></teamCard>
        </div>
      </div>
    </div>

    <!-- Footer -->
    <Footer></Footer>
  </div>
</template>

<script>
import Carousel from './components/Carousel.vue'
import Footer from './components/Footer.vue'
import ImageText from './components/ImageText.vue'
import NewsSection from './components/NewsSection.vue'
import Services from './components/Services.vue'
import TeamCard from './components/TeamCard'

export default {
  name: 'App',
  components: {
    NewsSection,
    TeamCard,
    ImageText, 
    Carousel,
    Services,
    Footer,
  },
  data(){
    return{
      Team:[
      {
        codigo: 1,
        nombre: "Sebastian",
        descripcion: "Estudiante de Ingeneria de Control del Politecnico en Medellin.",
        rol: "Desarrollo TeamCard",
        image: 'https://imgur.com/Ez4ovbj.jpg'
      },
      {
        codigo: 2,
        nombre: "Ruben",
        descripcion: "Ingeniero de Petróleos Universidad Industrial de Santander.",
        rol: "Desarrollo News",
        image: 'https://imgur.com/xbKw2jJ.jpg'
      },
      {
        codigo: 3,
        nombre: "Estefania",
        descripcion: "Estudiante primer semestre de Ingenería de sistemas Universidad.",
        rol: "Desarrollo Header & Footer",
        image: 'https://imgur.com/2OykPDS.jpg'
      },
      {
        codigo: 4,
        nombre: "Alejandro",
        descripcion: "Estudiante de ingeniería industrial en la Universidad de Antioquia",
        rol: "Desarrollo Services",
        image: 'https://imgur.com/S3pXvoH.jpg'
      }
    ]
    }
  }
  
}

</script>


