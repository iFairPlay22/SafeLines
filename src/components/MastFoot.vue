<template>
  <v-bottom-navigation
    app
    background-color="white"
    color="black"
    dark
    horizontal
    scroll-threshold="0"
    hide-on-scroll
  >
    <v-btn v-for="({ title, icon, link }, i) in items" :key="i" @click="redirect(link)">
      <span class="subtitle-1 black--text">{{ title }}</span>
      <!-- black -->
      <v-icon class="black--text">{{ icon }}</v-icon>
      <!-- black -->
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
export default {
  name: "MastFoot",
  data() {
    return {
      items: [
        {
          title: "Linkedin",
          icon: "mdi-linkedin",
          link: ""
        },
        {
          title: "Youtube",
          icon: "mdi-youtube",
          link: "https://www.youtube.com/channel/UCMe_TV5aa4S_bsMBj0tcDCA"
        },
        {
          title: "Email",
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
