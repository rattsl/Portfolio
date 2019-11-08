<template>
  <v-app class="grey lighten-4">
      <v-row
      align="center"
      justify="center"
      >
        <h1 class="display-3 font-weight-bold ul my-12 d-inline-block">Experience</h1>
      </v-row>
      <v-row
      align="center"
      justify="center"
      class="ma-10 pa-10"
      >

      <v-lazy
        :options="{
          threshold: 1
        }"
        transition="scale-transition"
      >
        <v-timeline dense>

        <v-timeline-item>
            <v-card class="elevation-2" max-width="600px">
                <v-card-title class="headline">Geeksalon iOS開発コース</v-card-title>
                <v-card-subtitle>2019年1月~2019月4月</v-card-subtitle>
                <v-card-text>
                    ミクロ経済学クイズアプリを開発。教材による学習から始まり企画、開発、LTなど一連の流れを初めて体験し、アプリ開発の楽しさを経験しました。
                </v-card-text>
                <v-divider></v-divider>
                <v-card-actions>
                <v-btn tile class="pa-2">Work</v-btn>
                </v-card-actions>
            </v-card>
        </v-timeline-item>

        <v-timeline-item>
            <v-card class="elevation-2" max-width="600px">
                <v-card-title class="headline">Geeksalon WebExpertコース</v-card-title>
                <v-card-subtitle>2019年6月~2019年9月</v-card-subtitle>
                <v-card-text>
                    Githubを使って動物自己診断アプリを共同開発を経験しました。主にUI/UXのデザインやコンテンツなどを担当しました。
                </v-card-text>
                <v-divider></v-divider>
                <v-card-actions>
                <v-btn tile class="pa-2">Work</v-btn>
                </v-card-actions>
            </v-card>
        </v-timeline-item>

         <v-timeline-item>
            <v-card class="elevation-2" max-width="600px">
                <v-card-title class="headline">学校法人角川ドワンゴ学園 インターン</v-card-title>
                    <v-card-subtitle>2019年9月~</v-card-subtitle>
                <v-card-text>
                    角川ドワンゴ学園N中等部にてプログラミングTAとして勤務。教材作成やプログラミング授業のメインファシリテータなどを行なっています。
                </v-card-text>
            </v-card>
        </v-timeline-item>
        </v-timeline>

      </v-lazy>
        
      </v-row>
  </v-app>
</template>

<script>
export default {

}
</script>

<style>

</style>