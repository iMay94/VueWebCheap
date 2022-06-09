<template>
  <v-container >

   <br><br><br><br>
    <v-row>
      <v-col
        cols="12"
        sm="3"
      >

      <v-card
        elevation="2"
        width="400"
      >
        <v-img
         height="300px"
         src="https://www.eleconomista.com.mx/__export/1652322654133/sites/eleconomista/img/2020/12/15/tulum_shutterstock_12255288.jpg_1093282975.jpg"

       >
        <v-container
          class=" white--text mt-8"
        >

        </v-container>
       </v-img>
       <v-card-title>
          Tulum - Hotel Zone
        </v-card-title>
        <v-card-subtitle>
          Private Van - 1 to 5 passengers
        </v-card-subtitle>


            <v-stepper v-model="e1">
              <v-stepper-header>
                <v-stepper-step
                  :complete="e1 > 1"
                  step="1"
                >
                  Type Service
                </v-stepper-step>

                <v-divider></v-divider>

                <v-stepper-step
                  :complete="e1 > 2"
                  step="2"
                >
                  Name of step 2
                </v-stepper-step>

                <v-divider></v-divider>

                <v-stepper-step step="3">
                  Name of step 3
                </v-stepper-step>
              </v-stepper-header>

              <v-stepper-items>
                <v-stepper-content step="1">
                  <v-card
                    elevation="0"
                    height="auto"
                  >

                    <v-container>
                      <v-row>

                        <v-col
                          cols="12"
                          sm="6"
                          class="text-center"
                        >

                          <h4>$75.00 USD</h4>
                          <br>
                          <v-btn
                            style="width: 100%;"
                            outlined
                            color="indigo"
                             @click="e1 = 2"
                          >
                            One Way
                          </v-btn>

                        </v-col>

                        <v-col
                          cols="12"
                          sm="6"
                          class="text-center"
                        >

                          <h4>$75.00 USD</h4>
                          <br>
                          <v-btn
                            style="width: 100%;"
                            outlined
                            color="indigo"
                             @click="e1 = 2"
                          >
                            Round Trip
                          </v-btn>

                        </v-col>

                      </v-row>
                      <br>
                    </v-container>

                  </v-card>
                </v-stepper-content>

                <v-stepper-content step="2">
                  <v-card
                    elevation="0"
                    height="auto"
                  >

                    <v-container fluid>


                          <v-select

                            :items="items"
                            label="Outlined style"
                            outlined
                            dense
                          ></v-select>

                          <v-autocomplete
                            dense
                            outlined
                            :items="states"
                            item-text="name"
                            filled
                            solo
                          ></v-autocomplete>


                    </v-container>

                  </v-card>


                </v-stepper-content>

                <v-stepper-content step="3">
                  <v-card
                    class="mb-12"
                    color="grey lighten-1"
                    height="200px"
                  ></v-card>

                  <v-btn
                    color="primary"
                    @click="e1 = 1"
                  >
                    Continue
                  </v-btn>

                  <v-btn text>
                    Cancel
                  </v-btn>
                </v-stepper-content>
              </v-stepper-items>
            </v-stepper>



      </v-card>


      </v-col>
      <v-col
      cols="12"
      sm="3"
      >
        <v-card
          elevation="2"
          width="400"
        >
          <v-img
           height="300px"
           src="https://www.eleconomista.com.mx/__export/1652322654133/sites/eleconomista/img/2020/12/15/tulum_shutterstock_12255288.jpg_1093282975.jpg"

         >
          <v-container
            class=" white--text mt-8"
          >

          </v-container>
         </v-img>
         <v-card-title>
            Tulum - Hotel Zone
          </v-card-title>
          <v-card-subtitle>
            Private Van - 1 to 5 passengers
          </v-card-subtitle>
          <v-container>
            <v-row>
              <v-col
                cols="12"
                sm="6"
              >
              <v-btn
                style="width:100%;"

                outlined
                color="indigo"
              >
                One Way
              </v-btn>
              </v-col>
              <v-col
                cols="12"
                sm="6"
              >
              <v-btn
                style="width:100%;"

                outlined
                color="indigo"
              >
                Round Trip
              </v-btn>
              </v-col>
            </v-row>
          </v-container>

        </v-card>
      </v-col>
      <v-col
      cols="12"
      sm="3"
      >
      <v-card
        elevation="2"
        width="400"
      >
        <v-img
         height="300px"
         src="https://www.eleconomista.com.mx/__export/1652322654133/sites/eleconomista/img/2020/12/15/tulum_shutterstock_12255288.jpg_1093282975.jpg"

       >
        <v-container
          class=" white--text mt-8"
        >

        </v-container>
       </v-img>
       <v-card-title>
          Tulum - Hotel Zone
        </v-card-title>
        <v-card-subtitle>
          Private Van - 1 to 5 passengers
        </v-card-subtitle>
        <v-container>
          <v-row>
            <v-col
              cols="12"
              sm="6"
            >
            <v-btn
              style="width:100%;"

              outlined
              color="indigo"

            >
              One Way
            </v-btn>
            </v-col>
            <v-col
              cols="12"
              sm="6"
            >
            <v-btn
              style="width:100%;"

              outlined
              color="indigo"
            >
              Round Trip
            </v-btn>
            </v-col>
          </v-row>
        </v-container>

      </v-card>
      </v-col>
      <v-col
      cols="12"
      sm="3"
      >
      <v-card
        elevation="2"
        width="400"
      >
        <v-img
         height="300px"
         src="https://www.eleconomista.com.mx/__export/1652322654133/sites/eleconomista/img/2020/12/15/tulum_shutterstock_12255288.jpg_1093282975.jpg"

       >
        <v-container
          class=" white--text mt-8"
        >

        </v-container>
       </v-img>
       <v-card-title>
          Tulum - Hotel Zone
        </v-card-title>
        <v-card-subtitle>
          Private Van - 1 to 5 passengers
        </v-card-subtitle>

        <v-container>
          <v-row>
            <v-col
              cols="12"
              sm="6"
            >
            <v-btn
              style="width:100%;"

              outlined
              color="indigo"
            >
              One Way
            </v-btn>
            </v-col>
            <v-col
              cols="12"
              sm="6"
            >
            <v-btn
              style="width:100%;"

              outlined
              color="indigo"
            >
              Round Trip
            </v-btn>
            </v-col>
          </v-row>
        </v-container>

      </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    data () {
      return {
        e1: 1,
        states: [
         { name: 'Florida', abbr: 'FL', id: 1 },
         { name: 'Georgia', abbr: 'GA', id: 2 },
         { name: 'Nebraska', abbr: 'NE', id: 3 },
         { name: 'California', abbr: 'CA', id: 4 },
         { name: 'New York', abbr: 'NY', id: 5 },
       ],
      }
    },
  }
</script>
