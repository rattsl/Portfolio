<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span class="font-weight-light">PORTFOLIO</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        text
        href="#"
        target="_blank"
      >
        <span class="mr-2">TOP</span>
      </v-btn>
      <v-btn
        text
        href="#"
        target="_blank"
      >
        <span class="mr-2">ABOUT</span>
      </v-btn>
      <v-btn
        text
        href="#"
        target="_blank"
      >
        <span class="mr-2">PROFILE</span>
      </v-btn>
      <v-btn
        text
        href="#"
        target="_blank"
      >
        <span class="mr-2">PORTFOLIO</span>
        <!-- ここでポップアップでEXPERIENCEとWORKSとSKILLASETTSの3つをだす -->
      </v-btn>
      <v-btn
        text
        href="#"
        target="_blank"
      >
        <span class="mr-2">CONTACT</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <Top/>
      <About/>
      <Profile/>
      <Portfolio/>
      <contact/>
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
import Portfolio from '@/containers/Portfolio.vue'
import Contact from '@/containers/Contact.vue'


export default {
  name: 'App',
  components: {
    Top,
    About,
    Profile,
    Portfolio,
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
