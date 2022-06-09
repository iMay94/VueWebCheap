<template>
  <v-container>

    <br>
    <v-sheet
    color="white"
    elevation="3"

    >
      <v-container>
      <v-form
      ref="form"
      v-model="valid"
      lazy-validation
      >

          <div class="text-lg-h6 text--secondary">
           <br>
            Book your transfer
          </div>
          <br>
          <v-autocomplete
            outlined
            v-model="select"
            :loading="loading"
            :items="items"
            :search-input.sync="search"
            cache-items
            class="mx-5"
            flat
            hide-no-data
            hide-details
            label="Select your hotel"
          ></v-autocomplete>
          <br>
          <v-select
            :items="items"
            class="mx-5"
            label="Type service"
            outlined
          ></v-select>
          <v-text-field
            class="mx-5"
            v-model="numberValue"
            hide-details
            outlined
            type="number"
          />
          <br>
          <v-btn
            class="mx-5"
          >
            Block Button
          </v-btn>
          <br>
            <br>
      </v-form>
      </v-container>
    </v-sheet>

  </v-container>
</template>
<script>
  export default {
    data () {
      return {
        loading: false,
        items: ['Round Trip', 'One Way - Arrival', 'One Way - Departure'],
        search: null,
        select: null,
        states: [
          'Alabama',
          'Alaska',
          'American Samoa',
          'Arizona',
          'Arkansas',
          'California',
          'Colorado',
          'Connecticut',
          'Delaware',
          'District of Columbia',
          'Federated States of Micronesia',
          'Florida',
          'Georgia',
          'Guam',
          'Hawaii',
          'Idaho',
          'Illinois',
          'Indiana',
          'Iowa',
          'Kansas',
          'Kentucky',
          'Louisiana',
          'Maine',
          'Marshall Islands',
          'Maryland',
          'Massachusetts',
          'Michigan',
          'Minnesota',
          'Mississippi',
          'Missouri',
          'Montana',
          'Nebraska',
          'Nevada',
          'New Hampshire',
          'New Jersey',
          'New Mexico',
          'New York',
          'North Carolina',
          'North Dakota',
          'Northern Mariana Islands',
          'Ohio',
          'Oklahoma',
          'Oregon',
          'Palau',
          'Pennsylvania',
          'Puerto Rico',
          'Rhode Island',
          'South Carolina',
          'South Dakota',
          'Tennessee',
          'Texas',
          'Utah',
          'Vermont',
          'Virgin Island',
          'Virginia',
          'Washington',
          'West Virginia',
          'Wisconsin',
          'Wyoming',
        ],
      }
    },
    watch: {
      search (val) {
        val && val !== this.select && this.querySelections(val)
      },
    },
    methods: {
      querySelections (v) {
        this.loading = true
        // Simulated ajax query
        setTimeout(() => {
          this.items = this.states.filter(e => {
            return (e || '').toLowerCase().indexOf((v || '').toLowerCase()) > -1
          })
          this.loading = false
        }, 500)
      },
    },
  }
</script>
