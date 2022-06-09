<template>
  <v-parallax
    dark
    src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
    style="height: 650px;"
  >
    <v-row
      align="center"
      justify="center"
    >
      <v-col
        class="text-center"
        cols="12"
      >

        <Main/>
        <v-container>
          <v-row no-gutters>
            <v-col
              cols="12"
              sm="4"
            >

            </v-col>
            <v-col
              cols="12"
              sm="4"
            >

            </v-col>

            <v-col
              cols="12"
              sm="3"
            >


              <BookPanel/>

            </v-col>

          </v-row>
        </v-container>

      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>

  import Main from './Main'
  import BookPanel from './BookPanel'


  export default {
    name: 'App',
    components: {
      Main,
      BookPanel
    },

    data: () => ({
      //
    }),
  };
</script>
