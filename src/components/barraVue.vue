<template>
  <b-navbar toggleable="lg" class="navbar-horizontal shadow-lg">
    <b-navbar-brand>
      <b-icon icon="person-badge-fill" variant="dark"></b-icon>
      <span title="name" class="font-weight-bold mt-auto ml-3"> Nicolas Rodriguez Hilarion</span>
    </b-navbar-brand>

    <b-navbar-nav>
      <b-nav-item href="#" class="mt-auto ml-auto">
        <b-badge variant="white">
          <span title="ocupation" class="text-secondary">Backend Engineer / T-Shaped </span>
          <b-icon variant="secondary" icon="code-slash"></b-icon></b-badge
      ></b-nav-item>
      <b-nav-item
        href="https://goo.gl/maps/Qvpojnycmj3teTx76"
        class="mt-auto ml-auto"
      >
        <b-badge variant="white">
          <span title="location" class="text-secondary">Colombia. Bogotá, D.C </span>
          <b-icon
            variant="secondary"
            scale="0.9"
            icon="geo-alt-fill"
          ></b-icon></b-badge
      ></b-nav-item>
    </b-navbar-nav>

    <b-navbar-nav class="ml-auto display-inline">
      <b-nav-item title="github" :href="github"
        ><b-icon icon="github" variant="dark"></b-icon
      ></b-nav-item>
      <b-nav-item :href="phone"
        ><b-icon icon="telephone-fill" variant="dark"></b-icon
      ></b-nav-item>
      <b-nav-item :href="mail"
        ><b-icon icon="envelope-fill" variant="dark"></b-icon
      ></b-nav-item>
      <b-nav-item :href="linkedin"
        ><b-icon icon="linkedin" variant="dark"></b-icon
      ></b-nav-item>
      <b-nav-item :href="portfolio"
        ><b-icon icon="folder-fill" variant="dark"></b-icon
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
                 phone: 'https://wa.me/573118913227',
                 mail: 'mailto:nicolasrhila@gmail.com',
                 linkedin: 'https://www.linkedin.com/in/nicolas-rodriguez-hilarion-765b321b3',
                 portfolio: 'https://nicolasrodriguezh.github.io/vue-pages/'
          }
      }
};
</script>
