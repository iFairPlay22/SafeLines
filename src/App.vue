<template>
  <v-app>
    <mast-head />

    <v-content>
      <router-view />
    </v-content>

    <mast-foot />
  </v-app>
</template>

<script>
import MastHead from "./components/MastHead";
import MastFoot from "./components/MastFoot";

export default {
  name: "App",
  components: {
    MastHead,
    MastFoot
  },
  data() {
    return {
      links: [
        {
          name: "About Me",
          link: "#about"
        },
        {
          name: "Last Songs",
          link: "#music"
        },
        {
          name: "Albums",
          link: "#playlist"
        },
        {
          name: "Contact",
          link: "#contact"
        }
      ]
    };
  }
};
</script>

<style lang="scss">
@import "~vuetify/src/styles/styles.sass";

.custom-title {
  font-size: 2.5rem !important;
}

.custom-bar-title {
  font-size: 2.5rem !important;
}

@media #{map-get(
    $display-breakpoints,
    "xs-only"
  )} {
  .custom-title {
    font-size: 2rem !important;
  }

  .custom-bar-title {
    font-size: 1.2rem !important;
  }
}
</style>
