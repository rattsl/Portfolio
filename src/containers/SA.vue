<template>
  <v-app>
      <v-container class="mb-10">
        <v-row
        align="center"
        justify="center"
        class="my-10"
        >
            <h1 class="display-3 font-weight-bold ul my-12 d-inline-block">Skill-Assets</h1>
        </v-row>
        <v-row
        align="center"
        justify="center"
        class="my-10"
        >
        <h3>開発に使用した言語です。開発に当てた時間や理解度など、<br>主観で評価しているので悪しからず。</h3>
        </v-row>

        <v-lazy
                :options="{
                threshold: 1
                }"
                transition="scale-transition"
            >

        <v-sheet dense class="pa-8">

        <v-row
            class="my-10"        
        >
            <v-col>
                <h2 class="text-center ma-3">Front</h2>
                <h3 class="mt-4">
                    HTML/CSS
                </h3>
                <v-progress-linear
                color="red lighten-2"
                buffer-value="0"
                value="30"
                height="17"
                stream
                >
                </v-progress-linear>
                <h3 class="mt-4">
                    JavaScript
                </h3>
                <v-progress-linear
                color="red lighten-2"
                buffer-value="0"
                value="30"
                height="17"
                stream
                >
                </v-progress-linear>
                <h3 class="mt-4">
                    Vue.js
                </h3>
                <v-progress-linear
                color="red lighten-2"
                buffer-value="0"
                value="40"
                height="17"
                stream
                ></v-progress-linear>

            </v-col>
            <v-col>
                <h2 class="text-center ma-3">Native</h2>
                <h3 class="mt-4">
                    Swift
                </h3>
                <v-progress-linear
                buffer-value="0"
                value="40"
                height="17"
                stream
                color="cyan"
                ></v-progress-linear>
            </v-col>
            <v-col>
                <h2 class="text-center ma-3">DevOps</h2>
                <h3 class="mt-4">
                    Git/Github
                </h3>
                <v-progress-linear
                buffer-value="0"
                value="40"
                height="17"
                stream
                color="orange"
                ></v-progress-linear>
                <h3 class="mt-4">
                    Firebase
                </h3>
                <v-progress-linear
                buffer-value="0"
                value="20"
                height="17"
                stream
                color="orange"
                ></v-progress-linear>
            </v-col>
        </v-row>
        </v-sheet>

        </v-lazy>

    </v-container>
  </v-app>
</template>

<script>
export default {
    
}
</script>

<style>
.fix{
    position: relative;
    top: 5px;
}

</style>