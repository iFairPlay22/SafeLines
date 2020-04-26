<template>
  <div>
    <v-card flat color="transparent" class="d-flex align-center justify-center my-3">
      <v-card-title class="display-2 text-center">Our team</v-card-title>
    </v-card>

    <v-card flat color="transparent" class="d-flex flex-row justify-center flex-wrap">
      <v-card
        color="transparent"
        v-for="({ img, name, role, linkedin }, i) in team"
        :key="i"
        class="ma-3"
      >
        <v-img :src="img" max-width="250px" max-height="200px" />
        <v-card-title
          class="indigo--text text--accent-4 d-flex justify-center ma-0 pa-0 pt-2"
        >{{ name }}</v-card-title>
        <v-card-text class="text-center ma-0 pa-0 pb-1">{{ role }}</v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>

          <v-btn icon v-if="linkedin != ''" @click="redirect(linkedin)">
            <v-icon>mdi-linkedin</v-icon>
          </v-btn>

          <v-btn icon>
            <v-icon>mdi-share-variant</v-icon>
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-card>
  </div>
</template>

<script>
export default {
  name: "Team",
  data() {
    return {
      team: [
        {
          img: require("@/assets/team/jaillon.jpg"),
          name: "Thomas Jaillon",
          role: "Engineer student at ESIEE PARIS",
          linkedin: "https://www.linkedin.com/in/thomas-jaillon-5244751a1"
        },
        {
          img: require("@/assets/team/sergent.jpeg"),
          name: "Pierre Sergent",
          role: "Business Student at ESSCA Paris",
          linkedin: "https://www.linkedin.com/in/pierre-sergent-935358177/"
        },
        {
          img: require("@/assets/team/bouquet.jpeg"),
          name: "Ewen Bouquet",
          role: "Engineer student at ESIEE PARIS",
          linkedin: "https://www.linkedin.com/in/ewen-bouquet/"
        },
        {
          img: require("@/assets/logo2.png"),
          name: "Dao Jonathan",
          role: "Engineer student at ESIEE PARIS",
          linkedin: ""
        },
        {
          img: require("@/assets/team/sautiere.jpg"),
          name: "Jade Sautiere",
          role: "Speech therapist student at Paris",
          linkedin: ""
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

<style>
</style>