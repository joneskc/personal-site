<template>
  <v-app id="app" dark>
    <v-toolbar id="header">
      <v-toolbar-title>Keith Jones</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn class="navBtn" flat>About</v-btn>
        <v-btn class="nav-btn" flat>Resumé</v-btn>
        <v-btn class="nav-btn" flat>Projects</v-btn>
        <v-btn class="nav-btn" flat>Contact</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-parallax
      height="1000"
      dark
      src="./static/denver-skyline.jpg"
    >
      <v-layout
        align-center
        column
        justify-center
      >
      <v-container height="1000">
        <router-view />
        <img src="../static/headshot.jpg" alt="Keith Jones">
        <h1 class="display-2 font-weight-thin mb-3">Vuetify.js</h1>
        <h4 class="subheading">Build your application today!</h4>
      </v-container>
      </v-layout>
    </v-parallax>
    <v-container>
      <h1>heres all the shit ill say, maybe put some projects in here</h1>
    </v-container>
  </v-app>
</template>

<script>
import Parallax from 'vue-parallaxy'
import Vuetify from 'vuetify'

export default {
  name: 'app',
  components: {
    Parallax
  },
  methods: {
    onSelected(idx) {
      console.log(`selected index: ${idx}`);
    },
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 5000;
  /* margin-top: 60px; */
}
#header {
  background-color: #5CDB95;
  color: #05386B;
  position: fixed;
  top: 0px;
}
.navBtn {
  color: #05386B;
}
</style>
