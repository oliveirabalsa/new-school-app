<template>
<div >
  <v-app id="inspire">
    <v-app-bar
      app
     
      
      
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="./assets/logo.png"
          transition="scale-transition"
          width="60"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        target="_blank"
        text
      >
        <span class="mr-2"></span>
        <v-icon>fas fa-list</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content class="back">
      <About/>
    </v-content>
    <Footer/>
  </v-app>
  </div>
</template>

<script>
import About from './components/About';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    About,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>
<style>


#inspire{
  background: none;
}

.back{
  background-image: url(./assets/paraisopolis1.png); 
  background-size: cover
}
</style>
