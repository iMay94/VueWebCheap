<template>
  <v-app>
    <v-main>
      <Top/>
      <Catalogue/>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <br>
      <Footer/>
    </v-main>
  </v-app>
</template>

<script>
//import Menu  from './components/Menu';
import Top from './components/Top'
import Footer from './components/Footer'
import Catalogue from './components/Catalogue'

export default {
  name: 'App',
  components: {
    Top,
    Footer,
    Catalogue
  },

  data: () => ({
    //
  }),
};
</script>
