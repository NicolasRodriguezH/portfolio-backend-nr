<template>
  <b-container>
    <b-card variant="dark" class="container shadow-lg rounded mt-5" style="background-color: rgba(0, 0, 0, 0.5);">
      <span class="font-weight-bold" style="color: #f8f9fa; opacity: 0.8;">Technologies of use</span> <br />
      <span class="text-secondary">(move the mouse or touch the icons)</span>

      <hr />

      <div class="img-content">
        <i
          class="_icons m-2"
          v-for="(svg, index) in items"
          :id="'icon:' + index"
          :key="index"
          v-on:mouseover="colorful('icon:' + index)"
          v-on:mouseleave="colorless('icon:' + index)"
          :class="svg.data"
        ></i>
      </div>
    </b-card>
  </b-container>
</template>

<script>
export default {
  name: "tecnologiesVue",
  data() {
    return {
      items: [
        { data: "devicon-unity-original" },
        { data: "devicon-csharp-plain"},
        { data: "devicon-go-plain" },
        { data: "devicon-php-plain" },
        { data: "devicon-laravel-plain" },
        { data: "devicon-mysql-plain" },
        { data: "devicon-vuejs-plain" },
        { data: "devicon-nodejs-plain" },
        { data: "devicon-typescript-plain" },
        /* 
        { data: "devicon-javascript-plain" },
        { data: "devicon-mongodb-plain" },
        { data: "devicon-git-plain" },
        { data: "devicon-html5-plain" },
        { data: "devicon-css3-plain" },
        { data: "devicon-linux-plain" },
        { data: "devicon-arduino-plain" },
        { data: "devicon-adonisjs-plain" }, */
      ],
    };
  },
  methods: {
    colorful(id) {
      document.getElementById(id).classList.add("colored");
    },
    colorless(id) {
      document.getElementById(id).classList.remove("colored");
    },
  },
};
</script>

<style scoped>
._icons {
  font-size: 40px;
  transition: 500ms;
}
._icons:hover {
  font-size: 60px;
  transition: 500ms;
}
</style>
