<template>
  <v-app>
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
      <v-col class="text-center mb-6" >
          <h1 class="display-3 font-weight-bold ul d-inline-block">About</h1>
          <h3 class="pa-4">このページは駆け出しエンジニアである僕がどういった<br>人物か、どんなものを制作してきたのかを紹介するページです。<br>このページに訪れたあなたと一緒に、僕の人生について少しでも共有できたら幸いです。</h3>
      </v-col>
          </v-lazy>
  </v-row>
  </v-app>  
</template>

<script>
export default {
}
</script>
