<template>
<v-app>
<v-container>
  <v-row
  align="center"
  justify="center"
  class="text-center my-10 py-10"
  >
    <h1 class="display-3 font-weight-bold ul">Works</h1>
  </v-row> 
  <v-row>
      <v-col
        align="center"
        justify="center"
      >
      <h3>ここでは制作物やジョインしたプロダクトの紹介をします。<br>まだ制作段階のものがあるので随時追加していきます。</h3>
      </v-col>
  </v-row>

  <v-lazy
        :options="{
          threshold: 1
        }"
        transition="scale-transition"
      >
  
    <v-slide-group
      v-model="model"
      class="ma-8 py-10"
      active-class="success"
      show-arrows
    >
      <v-slide-item
        v-for="card in cards"
        :key="card.date"
        :name="card.name"
        :language="card.language"
        :explain="card.explain"
      >
        <v-card
            class="ma-5"
            min-width="300"
            elevation="8"
        >
          <v-row
            align="center"
            justify="center"
          >
           <v-card-text>
            <div>{{ card.date }}</div>
            <p class="display-1 text--primary">
                {{ card.name }}
            </p>
            <p>{{ card.language }}</p>
            <div class="text--primary">
                {{ card.explain }}
            </div>
            </v-card-text>
            <v-divider></v-divider>
            <v-card-actions>
            <v-btn
                text
                color="deep-purple accent-4"
            >
                Show detail
            </v-btn>
            </v-card-actions>
          </v-row>
        </v-card>
      </v-slide-item>
    </v-slide-group>

  </v-lazy>

</v-container>
</v-app>  
</template>

<script>

export default {
  data () {
      return {
          cards: [
          {
              date: 'DATE',
              name: 'PRODUCT NAME',
              language: 'LANGUAGE',
              explain: 'OUTLINE',
          },
          {
              date: '2019年4月',
              name: 'ミクロ経済学入門',
              language: 'Swift',
              explain: 'hoge',
          },
          {
              date: '2019年9月',
              name: 'Identimal',
              language: 'Vue.js Firebase',
              explain: 'hogehoge'
          },
          {
              date: '2019年11月',
              name: 'Portfolio',
              language: 'Vue.js Vuetify',
              explain: 'hogehogehoge',
          },
          {
              date: '2019年11月',
              name: 'かっこいい垣内勇人',
              language: 'Node.js',
              explain: 'hogeeeeeeeeeeeeee',
          }
          ],
          model: null,
      }
  }

}
</script>