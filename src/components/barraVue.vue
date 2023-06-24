<template>
  <b-navbar toggleable="lg" class="navbar-horizontal shadow-lg fixed-top bg-gray" style="background-color: rgba(0, 0, 0, 0.5); color: #f8f9fa; opacity: 0.8;">
    
    <b-navbar-brand>
      <b-icon icon="person-badge-fill" style="color: #f8f9fa; opacity: 0.8;"></b-icon>
      <span title="name" class="font-weight-bold mt-auto ml-3" style="color: #f8f9fa; opacity: 0.8;"> Nicolas Rodriguez H.</span>
    </b-navbar-brand>

    <b-navbar-nav>
      <b-nav-item href="https://nicolasrodriguezh.itch.io/" class="mt-auto ml-auto" target="__blank">
        <b-badge variant="white">
          <span title="Games Portfolio" style="color: #f8f9fa; opacity: 0.8;"> Game Developer / T-Shaped </span>
          <b-icon variant="secondary" icon="code-slash"></b-icon></b-badge
      ></b-nav-item>

      <b-nav-item
        href="https://goo.gl/maps/Qvpojnycmj3teTx76"
        class="mt-auto ml-auto"
      >
        <b-badge variant="white">
          <span title="location" style="color: #f8f9fa; opacity: 0.8;">Colombia. Bogotá, D.C </span>
          <b-icon
            variant="secondary"
            scale="0.9"
            icon="geo-alt-fill"
          ></b-icon></b-badge
      ></b-nav-item>
    </b-navbar-nav>

    <b-navbar-nav class="ml-auto display-inline">

      <b-nav-item title="GitHub" :href="github"
        ><b-icon icon="github" style="color: #f8f9fa; opacity: 0.8;"></b-icon
      ></b-nav-item>
      
      <b-nav-item title="WhatsApp" :href="whatsapp"
        ><b-icon icon="whatsapp" style="color: #f8f9fa; opacity: 0.8;"></b-icon
      ></b-nav-item>
      
      <b-nav-item title="LinkedIn" :href="linkedin"
        ><b-icon icon="linkedin" style="color: #f8f9fa; opacity: 0.8;"></b-icon
      ></b-nav-item>

      <b-nav-item title="C.V" :href="portfolio" download target="__blank">
        <b-icon icon="folder-fill" style="color: #f8f9fa; opacity: 0.8;"></b-icon>      
      </b-nav-item>

      <!-- <b-nav-item title="Itch.io" :href="itchio"
        ><b-icon icon="folder-fill" variant="dark"></b-icon
      ></b-nav-item> -->

      <b-nav-item title="Mail" :href="mail"
        ><b-icon icon="envelope-fill" style="color: #f8f9fa; opacity: 0.8;"></b-icon
      ></b-nav-item>

    </b-navbar-nav>
  </b-navbar>
</template>

<script>
export default {
  name: "barraVue",
   data() {
          return {
                 github: 'https://github.com/NicolasRodriguezH',
                 whatsapp: 'https://wa.me/573118913227',
                 linkedin: 'https://www.linkedin.com/in/nicolas-rodriguez-hilarion-765b321b3',
                 portfolio: "NicolasRodriguez.H_CV.pdf",
                 //itchio: "https://nicolasrodriguezh.itch.io/",
                 mail: 'mailto:nicolasrhila@gmail.com',
          }
      },
};
</script>
