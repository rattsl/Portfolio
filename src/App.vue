<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span class="font-weight-light text-lowercase">rattsl.com</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        text
         @click="$vuetify.goTo('#top')"
      >
        <span class="mr-2">TOP</span>
      </v-btn>
      <v-btn
        text
        @click="$vuetify.goTo('#about')"
      >
        <span class="mr-2">ABOUT</span>
      </v-btn>
      <v-btn
        text
         @click="$vuetify.goTo('#profile')"
      >
        <span class="mr-2">PROFILE</span>
      </v-btn>
      <v-menu transition="scroll-y-transition">
        <template v-slot:activator="{ on }">
        <v-btn text class="ma-2" v-on="on">
          PORTFOLIO
        </v-btn>
        </template>
        <v-list>
        <v-list-item
          @click="$vuetify.goTo('#works')"
        >
          <v-list-item-title>WORKS</v-list-item-title>
        </v-list-item>
        <v-list-item
          @click="$vuetify.goTo('#experience')"
        >
          <v-list-item-title>EXPERIENCE</v-list-item-title>
        </v-list-item>
        <v-list-item
          @click="$vuetify.goTo('#sa')"
        >
          <v-list-item-title>SKILL-ASSETS</v-list-item-title>
        </v-list-item>
      </v-list>
      </v-menu> 
      <v-btn
        text
        @click="$vuetify.goTo('#contact')"
      >
        <span class="mr-2">CONTACT</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <Top id="top"/>
      <About id="about"/>
      <Profile id="profile"/>
      <Works id="works"/>
      <Experience id="experience"/>
      <SA id="sa"/>
      <contact id="contact"/>
    </v-content>
    <v-footer class="indigo">
    <v-spacer></v-spacer>
    <div>&copy; {{ new Date().getFullYear() }}</div>
  </v-footer>
  </v-app>
</template>

<script>

import Top from '@/containers/Top.vue'
import About from '@/containers/About.vue'
import Profile from '@/containers/Profile.vue'
import Works from '@/containers/Works.vue'
import Experience from '@/containers/Experience.vue'
import SA from '@/containers/SA.vue'
import Contact from '@/containers/Contact.vue'


export default {
  name: 'App',
  components: {
    Top,
    About,
    Profile,
    Works,
    Experience,
    SA,
    Contact,
  },
  data: () => ({
    //
  }),
};
</script>
<style>
.ul{
    border-bottom: 10px solid red;
}
</style>
