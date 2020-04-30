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
  background-color: red;
}

// h2 {
//   font-size: 1rem !important;
//   background-color: red;
// }

@media #{map-get(
    $display-breakpoints,
    "xs-only"
  )} {
  .custom-title {
    font-size: 2rem !important;
    background-color: green;
  }
  // h2 {
  //   font-size: 1.5rem !important;
  //   background-color: green;
  // }
}
</style>
