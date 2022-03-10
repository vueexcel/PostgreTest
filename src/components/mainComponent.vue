<template>
  <div>
    <v-container fluid blue-grey lighten-5>
      <v-row no-gutters>
        <v-col cols="1">
          <v-btn class="mx-6 mt-8" medium fab dark color="green">
            <v-icon dark> mdi-plus </v-icon>
          </v-btn>
        </v-col>
        <v-col cols="5">
          <leftContainer />
        </v-col>
        <v-col cols="5" class="mt-15">
          <rightUpperContainer />
          <rightMiddleContainer />
          <rightBottomContainer />
          <rightLastContainer />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import leftContainer from "./leftContainer.vue";
import rightUpperContainer from "./rightUpperContainer.vue";
import rightMiddleContainer from "./rightMiddleContainer.vue";
import rightBottomContainer from "./rightBottomContainer.vue";
import rightLastContainer from "./rightLastContainer.vue";

export default {
  name: "mainComponent",
  components: {
    leftContainer,
    rightMiddleContainer,
    rightUpperContainer,
    rightBottomContainer,
    rightLastContainer,
  },
};
</script>

<style>
</style>