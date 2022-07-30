<template>
  <b-card class="flex w-100 footer-vw" type="dark">
    <hr class="bg-dark" />
    <ul class="float-left mt-3 footer-list mt-4">
      <br />
      <a href="https://twitter.com/Nicolasrodh"><li><b-icon icon="twitter"></b-icon> Nicolasrodh</li></a>

      <div class="flex justify-center items-center text-center">
          <div
              class="font-general-regular text-lg text-ternary-dark dark:text-ternary-light"
            >
              &copy; {{ copyrightDate }}.
              <a
                href="https://github.com/NicolasRodriguezH/portfolio_nicolas_rh"
                target="__blank"
                class="font-general-medium hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500"
              >
                {{ projectName }}
              </a>
              . Developed by
              <a
                href="https://www.linkedin.com/in/nicolas-rodriguez-hilarion-765b321b3"
                target="__blank"
                class="font-general-medium text-secondary-dark dark:text-secondary-light uppercase hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500"
                >{{ author }}</a
              >
          </div>
      </div>
    </ul>

    <b-card no-body class="col-md-6 float-center mx-auto footer-vw">
      <a href='https://wa.me/573118913227'><strong class="text-white font-bold">Contact Me!</strong></a>
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
			projectName: 'Backend Developer Portfolio',
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