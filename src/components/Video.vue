<template>
  <v-container fluid>
    <v-layout row>
      <v-col cols="10" offset="1">
        <v-card
          flat
          color="transparent"
          class="d-flex flex-column align-center justify-center my-3"
        >
          <v-card-title class="display-2 text-center mb-5 text-break">Presentation</v-card-title>
          <div style="position: relative; width: 100%; height: 0; padding-bottom: 56.25%;">
            <iframe
              frameborder="0"
              allowfullscreen
              style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
              src="https://www.youtube.com/embed/qL9i0i784X8"
            ></iframe>
          </div>
        </v-card>
      </v-col>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "Video"
};
</script>