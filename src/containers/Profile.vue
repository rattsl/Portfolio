<template>
<v-app class="grey lighten-4">
    <v-container>

    <v-row
        align="end"
        justify="center" 
    >
            <h1 class="display-3 font-weight-bold ul my-12 d-inline-block">Profile</h1>
    </v-row>
    <v-row
        align="center"
        justify="center"    
    >
    <v-lazy
        :options="{
            threshold: .1
            }"
            transition="scale-transition"
    >   
        
        <v-col
        class="text-center"
        >

            <v-avatar size="300" class="elevation-12">
                <v-img src="@/assets/hayato.png">
                </v-img>
            </v-avatar>

            <h1 class="display-2 pa-6">Hayato Kakiuchi</h1>
            <h3>Web,iOS Developer</h3>
        </v-col>
    </v-lazy>
    </v-row>
    <v-row
        align="center"
        justify="center" 
    >
    <v-sheet class="grey lighten-4 my-5">
        <a href="https://twitter.com/rattsl/" target="_blank">
        <v-avatar size="50" class="mx-3">
            <v-img src="@/assets/Twitter.png"></v-img>
        </v-avatar>
        </a>
        <a href="https://www.facebook.com/profile.php?id=100033715362043" target="_blank">
        <v-avatar size="50" class="mx-3">
            <v-img src="@/assets/f_logo_RGB-Blue_144.png"></v-img>
        </v-avatar>
        </a>
        <a href="https://github.com/rattsl/" target="_blank">
        <v-avatar size="50" class="mx-3">
            <v-img src="@/assets/GitHub-Mark-120px-plus.png"></v-img>
        </v-avatar>
        </a>
    </v-sheet>
    </v-row>
    <v-row
        align="center"
        justify="center" 
    >
        <v-simple-table
         class="grey lighten-4 py-10"
         style="width: 600px"
         >
            <template v-slot:default>
                <tbody>
                    <tr v-for="item in profile" :key="item.name">
                    <td>{{ item.name }}</td>
                    <td>{{ item.value }}</td>
                    </tr>
                </tbody>
            </template>
        </v-simple-table>
    </v-row>
    <v-row
        align="center"
        justify="center" 
    >
        <v-stepper v-model="e6" class="grey lighten-4" vertical>

            <v-stepper-step :complete="e6 > 1" step="1">
                幼少期
            </v-stepper-step>
            <v-stepper-content step="1">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 2">Continue</v-btn>
            </v-stepper-content>

            <v-stepper-step :complete="e6 > 2" step="2">
                小学時代
            </v-stepper-step>
            <v-stepper-content step="2">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 3">Continue</v-btn>
            </v-stepper-content>

            <v-stepper-step :complete="e6 > 3" step="3">
                中学時代
            </v-stepper-step>
            <v-stepper-content step="3">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 4">Continue</v-btn>
            </v-stepper-content>

            <v-stepper-step :complete="e6 > 4" step="4">
                高校時代
            </v-stepper-step>
            <v-stepper-content step="4">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 5">Continue</v-btn>
            </v-stepper-content>

            <v-stepper-step :complete="e6 > 5" step="5">
                大学時代１
            </v-stepper-step>
            <v-stepper-content step="5">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 6">Continue</v-btn>
            </v-stepper-content>

            <v-stepper-step :complete="e6 > 6" step="6">
                大学時代２
            </v-stepper-step>
            <v-stepper-content step="6">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 7">Continue</v-btn>
            </v-stepper-content>

            <v-stepper-step step="7">
                現在
            </v-stepper-step>
            <v-stepper-content step="7">
            <v-card color="grey lighten-1" class="mb-12" min-height="400px" min-width="600px"></v-card>
            <v-btn color="primary" @click="e6 = 1">Continue</v-btn>
            </v-stepper-content>
        </v-stepper>
    </v-row>
    </v-container>
</v-app>  
</template>

<script>
export default {
data () {
      return {
        profile: [
          {
            name: '出身',
            value: '福井県',
          },
          {
            name: '在住',
            value: '東京都',
          },
          {
            name: '血液型',
            value: 'B型',
          },
          {
            name: '誕生日',
            value: '1996年 6月2日',
          },
          {
            name: '趣味',
            value: 'サッカー',
          },
          {
            name: '好きな言葉',
            value: '紆余曲折',
          },
          
        ],

        e6: 1,

      }
    }
}
</script>

<style>


</style>