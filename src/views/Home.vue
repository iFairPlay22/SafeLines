<template>
  <v-card class="d-flex flex-column justify-space-around align-center flex-wrap">
    <Issue />
    <Solution />
    <How />
    <Video />
    <Team />
  </v-card>
</template>

<script>
import Team from "@/components/Team.vue";
import Issue from "@/components/Issue.vue";
import Solution from "@/components/Solution.vue";
import How from "@/components/How.vue";
import Video from "@/components/Video.vue";

export default {
  name: "Home",
  components: {
    Team,
    Issue,
    Solution,
    How,
    Video
  },
  data() {
    return {};
  }
};
</script>
