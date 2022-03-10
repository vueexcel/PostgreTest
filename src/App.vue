<template>
  <v-app>
    <v-main>
      <mainComponent/>
    </v-main>
  </v-app>
</template>

<script>
import mainComponent from './components/mainComponent';

export default {
  name: 'App',

  components: {
    mainComponent,
  },

  data: () => ({
    //
  }),
};
</script>
