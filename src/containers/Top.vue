<template>
  <v-app>
  <v-parallax 
  src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
  height="600">
  <v-row
      align="center"
      justify="center"
    >
    <v-lazy
        :options="{
          threshold: 1
        }"
        transition="scale-transition"
      >
      <v-col class="text-center" cols="12">
        <h3 class="subheading">Creative Portfolio Site</h3>
        <h1 class="display-4 font-weight-bold mb-4">rattsl.com</h1>
      </v-col>
    </v-lazy>
    </v-row>
  </v-parallax>
  </v-app>
</template>

<script>
export default {

}
</script>

<style>

</style>