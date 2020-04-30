<template>
  <v-app-bar app color="white" light dense prominent scroll-threshold="0" hide-on-scroll>
    <v-card flat color="transparent" height="100%" class="d-flex justify-center align-center">
      <v-img height="60px" width="60px" src="@/assets/logo2.png"></v-img>
      <v-card-title class="black--text custom-title text-break">SafeLines</v-card-title>
    </v-card>
    <div class="flex-grow-1"></div>
    <v-btn icon v-for="({ icon, link }, i) in icons" :key="i" @click="redirect(link)">
      <v-icon class="black--text">{{ icon }}</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: "MastHead",
  data() {
    return {
      icons: [
        {
          icon: "mdi-linkedin",
          link: "https://www.linkedin.com/company/safelines"
        },
        {
          icon: "mdi-youtube",
          link: "https://www.youtube.com/channel/UCMe_TV5aa4S_bsMBj0tcDCA"
        },
        {
          icon: "mdi-email",
          link: ""
        }
      ]
    };
  },
  methods: {
    redirect(link) {
      if (link !== "") {
        window.open(link, "_blank");
      } else {
        window.location.href = "mailto:contact.safelines@gmail.com";
      }
    }
  }
};
</script>
