<template>
  <div class="d-flex justify-space-around align-center">
    <v-container fluid>
      <v-layout row>
        <v-col offset-lg="4" lg="4" offset-md="3" md="6" offset-sm="1" sm="10">
          <v-card
            min-width="250px"
            flat
            color="transparent"
            class="d-flex flex-column align-center justify-center my-3"
          >
            <v-card-title
              class="text-uppercase d-flex flex-row align-center justify-center text-break"
            >
              <div
                class="headline text-break"
                style="writing-mode: vertical-rl; transform: rotate(180deg); float: right;"
              >The</div>
              <div class="display-3 text-break">issue</div>
            </v-card-title>
            <v-card-text
              class="text-center body-1 text-break"
            >With social distancing being set by the government in all public areas, massive waiting lines were formed in front of every first-necessity shops at peak times, which causes overcrowding in shops and increases the risk of contamination. How can we do to reduce those waiting lines, avoid overcrowding and at the same time reduce the risk of contamination for both customers and employees?</v-card-text>
          </v-card>
        </v-col>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
export default { name: "Issue" };
</script>
