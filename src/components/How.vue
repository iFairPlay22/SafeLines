<template>
  <div class="d-flex justify-space-around align-center">
    <v-card flat color="transparent" class="d-flex flex-column align-center justify-center my-3">
      <v-card-title class="display-2 text-center mb-5">How it works?</v-card-title>
      <!--  -->
      <v-card flat color="transparent" class="d-flex flex-row justify-space-around flex-wrap">
        <v-card
          flat
          color="transparent"
          v-for="({ img, title, text }, i) in how"
          :key="i"
          class="d-flex flex-column justify-start align-center"
          max-width="20%"
          min-width="200px"
        >
          <v-img :src="img" max-width="200px" max-height="200px" />
          <v-card-title class="indigo--text text--accent-4 d-flex justify-center">{{ title }}</v-card-title>
          <v-card-text class="indigo--text text--accent-4 text-center body-1">{{ text }}</v-card-text>
        </v-card>
      </v-card>
      <!--  -->
    </v-card>
  </div>
</template>

<script>
export default {
  name: "How",
  data() {
    return {
      how: [
        {
          img: require("@/assets/how/1.png"),
          title: "Sign up on Safeline",
          text: ""
        },
        {
          img: require("@/assets/how/2.png"),
          title: "Find your favorite shops",
          text:
            "A map will be available on Safeline to see which stores are around you."
        },
        {
          img: require("@/assets/how/3.png"),
          title: "Get registered on a slot",
          text:
            "Once you get registered on a slot Safeline will provide you a QR code guaranteeing your reservation."
        },
        {
          img: require("@/assets/how/4.png"),
          title: "Show your QR code to enter the shop",
          text:
            "Confirm your attendance 15 minutes before the beginning of your time slot."
        }
      ]
    };
  }
};
</script>
