<template>
  <div id="app" :style="{ backgroundImage: 'url(' + require('@/assets/projects/gameDevBg.jpg') + ')', backgroundSize: 'cover', backgroundPosition: 'center' }">
    <barra-vue/>
  
    <div class="pt-5 pl-5">

      <div class="row">
        
        <div class="col-md-3">
          <ProfileVue/>
        </div>
        <div class="col-md-4">
        <LenguagesVue/> 
      </div>
      <div class="col-md-4">
        <TecnologiesVue/> 
      </div>
      
    </div>
    
  </div>

  <projects-vue/>
  
      <div class="col-md-12 pb-4 float-center mx-auto d-flex align-items">
       <about-vue/>
      </div>

  <FooterVue/>

  </div>
</template>

<script>
import BarraVue from './components/barraVue.vue'
import ProfileVue from './components/profileVue.vue'
import LenguagesVue from './components/lenguagesVue.vue'
import TecnologiesVue from './components/tecnologiesVue.vue'
import ProjectsVue from './components/projectsVue.vue'
import AboutVue from './components/aboutVue.vue'
import FooterVue from './components/footerVue.vue'

export default {
  name: 'App',
  components: {
    BarraVue,
    ProfileVue,
    LenguagesVue,
    TecnologiesVue,
    ProjectsVue,
    AboutVue,
    FooterVue
},
  /* data() {
    return {
      //backgroundImage: 'background-color: #E6F0FF',
      //transition: 'background-color 0.5s ease' // Transición de color suave

      backgroundImage: 'url(' + require('@/assets/projects/Adjust.png') + ')', backgroundSize: 'cover', backgroundPosition: 'center'

      // Ejemplo llamado en template HMTL
      //:style="{ 'background-image': backgroundImage }"
    };
}, */
}
</script>
