<template>
  <b-card class="flex w-100 footer-vw" type="dark">
    <hr class="bg-dark" />
    <ul class="float-left mt-3 footer-list mt-4">
      <br />
      <!-- <a href="https://twitter.com/Nicolasrodh"><li><b-icon icon="folder"></b-icon> Portfolio game devs</li></a> -->

      <div class="flex justify-center items-center text-center">
          <div
              class="font-general-regular text-lg text-ternary-dark dark:text-ternary-light"
            >
              &copy; {{ copyrightDate }}.
              <a
                href="https://nicolasrodriguezh.itch.io/"
                target="__blank"
                title="Games Portfolio"
                class="font-general-medium hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500"
              >
                {{ projectName }}
              </a>
              . Developed by
              <a
                href="NicolasRodriguez.H_CV.pdf"
                download
                title="C.V"
                class="font-general-medium text-secondary-dark dark:text-secondary-light uppercase hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500"
                >{{ author }}</a
              >
          </div>
      </div>
    </ul>

    <b-card no-body class="col-md-6 float-center mx-auto footer-vw">
      <a href='https://wa.me/573118913227'><strong class="font-bold" style="color: #f8f9fa; opacity: 0.8;">Contact Me On Whatsapp!</strong></a>
    </b-card>
    <hr class="bg-dark" />
  </b-card>
</template>

<script>

export default {
  name: "footerVue",
  data: () => {
    return {
      copyrightDate: new Date().getFullYear(),
			projectName: 'Game Dev Portfolio',
			author: 'Nicolas R.H',
    }
  },
};
</script>

<style scoped>
.footer-vw {
  background: rgb(27, 27, 27);
}
.footer-list {
  list-style: none;
  color: white;
}
.text {
  font-family: "Courier New", Courier, monospace;
}
</style>