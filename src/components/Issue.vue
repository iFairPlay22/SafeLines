<template>
  <div class="d-flex justify-space-around align-center">
    <v-card
      width="40%"
      flat
      color="transparent"
      class="d-flex flex-column align-center justify-center my-3"
    >
      <v-card-title
        class="text-uppercase d-flex flex-row align-center justify-center"
        style="min-width:300px;"
      >
        <div
          class="headline"
          style="writing-mode: vertical-rl; transform: rotate(180deg); float: right;"
        >The</div>
        <div class="display-3">issue</div>
      </v-card-title>
      <v-card-text
        class="text-center body-1"
      >With social distancing being set by the government in all public areas, massive waiting lines were formed in front of every first-necessity shops at peak times, which causes overcrowding in shops and increases the risk of contamination. How can we do to reduce those waiting lines, avoid overcrowding and at the same time reduce the risk of contamination for both customers and employees?</v-card-text>
    </v-card>
  </div>
</template>

<script>
export default { name: "Issue" };
</script>
