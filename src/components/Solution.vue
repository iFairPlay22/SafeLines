<template>
  <div class="d-flex justify-space-around align-center">
    <v-container fluid>
      <v-layout row>
        <v-col offset-lg="3" lg="6" offset-md="2" md="8" offset-sm="1" sm="10">
          <v-card
            min-width="250px"
            flat
            color="transparent"
            class="d-flex flex-row align-center justify-center flex-wrap my-3"
          >
            <v-card-title class="custom-title text-center text-break">Our magic solution</v-card-title>
            <v-card-text class="body-1 text-justify text-break">
              Safelines is an application that aims to limit waiting lines and
              regulate the number of people in the store with registration.
              Store owners propose time slots with a number of customers they
              think they can welcome in all safety. As a result both the
              customer experience and work conditions will be improve with a
              true feeling of security. Safeline will make shopping easier and
              safer for everyone.
            </v-card-text>
          </v-card>
        </v-col>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
export default { name: "Solution" };
</script>