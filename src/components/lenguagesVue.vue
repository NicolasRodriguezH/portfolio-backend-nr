<template>
  <b-container>
    <b-card variant="dark" class="shadow-lg rounded mt-5" style="background-color: rgba(0, 0, 0, 0.5);">
      <span class="font-weight-bold" style="color: #f8f9fa; opacity: 0.8;"> Percentage of use </span>
      <br />
      <span class="text-secondary"> (this does not represent the level) </span>
      <hr />
      <br />
      <div v-for="bar in bars" :key="bar.value" class="row mb-2">
        <div class="col-md-7">
          <b-badge class="text-white col-ms-1" variant="dark">{{
            bar.title
          }}</b-badge>
          <b-progress
            :value="bar.value"
            variant="secondary"
            striped
            animated="animated"
          ></b-progress>
        </div>
      </div>
      <br />
    </b-card>
  </b-container>
</template>
<script>
export default {
    name: 'lenguagesVue',
    data() {
        return {
            bars: [
                {title: "Unity", value: 89, variant: "primary"},
                {title: "C#", value: 89, variant: "primary"},
                //{title: "PHP", value: 30, variant: "danger"},
                {title: "MySQL", value: 60, variant: "primary"},
                //{title: "Laravel", value: 45, variant: "primary"},
                //{title: "GOlang", value: 30, variant: "primary"},
                //{title: "Vue", value: 35, variant: "success"},
                //{title: "TypeScript", value: 40, variant: "primary"},
                //{title: "JavaScript", value: 30, variant: "warning"},
            ]
        }
    }
}
</script>
