<template>
     <b-container class="mt-5 contenedor col-md-6" >
    <b-badge class="w-100 text-white font-weight-bolder mx-auto p-1" variant="dark">Projects</b-badge>
    <b-carousel    
        id="carousel"
        style="text-shadow: 0px 0px 5px black;"
        v-model="open_slide"
        :interval="0"
        controls
        indicators
        class="text-center"
    >
      <a :href="slides[open_slide].link">
         <b-carousel-slide
         v-for="(slide, index) in slides"
        :key="index"
        :caption="slide.caption"
        :img-src="slide.src"
        :id="slide.link"
        class="vtam"
        text="click to open GitHub or Itch.io"
     >   
     </b-carousel-slide>
      </a>
    </b-carousel>

    </b-container>

    
</template>

<script>
export default {
    name: 'projectsVue',
    data() {
        return {
            slides: [
                {caption: "The Last Crusade", src: require("../assets/projects/LastCrusadeImage.png"), link: "https://six-guys-productions.itch.io/the-last-crusade"},
                {caption: "DarkPairs", src: require("../assets/projects/FondoDarkPairs.jpg"), link: "https://sergtran.itch.io/dark-pair"},
                {caption: "GameJam Proyect", src: require("../assets/projects/GameJam1.png"), link: "https://rodrigo-c-v.itch.io/game-jam-run-for-food"},
                {caption: "Project Self-1 Game", src: require("../assets/projects/ProjectSelf.png"), link: "https://nicolasrodriguezh.itch.io/projectself"},
                
                {caption: "Laravel Autoadmin Blog", src: require("../assets/projects/footer.png"), link: "https://github.com/NicolasRodriguezH/blog-system-laravel-jetstream-personalized"},
                {caption: "GOlang API", src: require("../assets/projects/GoRoutes.png"), link: "https://github.com/NicolasRodriguezH/golang_api"},
                {caption: "NodeJS APIrestfull - Vue, Vuetify client", src: require("../assets/projects/addArticle.png"), link: "https://github.com/NicolasRodriguezH/apirest_nodejs"},
                //{caption: "CRUD NodeJS", src: require("../assets/projects/deleteRegister.png"), link: "https://github.com/NicolasRodriguezH/CRUD_NODEJS"},
                {caption: "SPA-Vue-vuetify-axios-apirestful-mysql", src: require("../assets/projects/registrationFormView.png"), link: "https://github.com/NicolasRodriguezH/SPA-Vue-vuetify-axios-apirestful-mysql"},
                //{caption: "Laravel CRUD Courses with", src: require("../assets/projects/filterCoursesView.png"), link: "https://github.com/NicolasRodriguezH/Web-app-dinamica-con-Livewire"},
                {caption: "Laravel Vue App-SPA", src: require("../assets/projects/modalAppSPA.png"), link: "https://github.com/NicolasRodriguezH/laravel-vue-SPA"},
                {caption: "Login JWT NodeJS", src: require("../assets/projects/tokenJwtLogin.png"), link: "https://github.com/NicolasRodriguezH/login_node_jwt"},
                {caption: "Basic BLockchain GOlang", src: require("../assets/projects/mine_block_route.png"), link: "https://github.com/NicolasRodriguezH/basic-blockchain-golang"},
            ],  
            open_slide: 0
        }
    }

}
</script>

<style>
.vtam {
   height:40vh;
   background: #292b2c;
 }
</style>