<template>
  <v-card flat color="transparent" class="d-flex justify-space-around align-center" width="60%">
    <v-card
      flat
      color="transparent"
      class="d-flex flex-column align-center justify-center my-3"
      width="100%"
    >
      <v-card-title class="display-2 text-center mb-5">Presentation</v-card-title>
      <iframe
        width="100%"
        src="https://www.youtube.com/embed/qL9i0i784X8"
        style="min-height: 450px"
      ></iframe>
    </v-card>
  </v-card>
</template>

<script>
export default {
  name: "Video"
};
</script>