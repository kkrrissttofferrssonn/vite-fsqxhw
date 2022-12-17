<script>
export default {
  data: () => ({ rating: 3 }),
};
</script>
<template>
  <!-- unplugin-vue-components auto import -->
  <v-app>
    <Header />
    <v-row justify="space-around">
      <v-icon size="large" color="green-darken-2"> mdi-domain </v-icon>

      <v-icon size="large" color="blue-darken-2"> mdi-message-text </v-icon>

      <v-icon size="large" color="purple-darken-2"> mdi-dialpad </v-icon>

      <v-icon size="large" color="teal-darken-2"> mdi-email </v-icon>

      <v-icon size="large" color="blue-grey-darken-2"> mdi-call-split </v-icon>

      <v-icon size="large" color="orange-darken-2">
        mdi-arrow-up-bold-box-outline
      </v-icon>
    </v-row>
    <v-container class="bg-surface-variant">
      <v-row justify="start">
        <v-col v-for="k in 2" :key="k" cols="4">
          <v-sheet class="pa-2 ma-2"> .justify-start </v-sheet>
        </v-col>
      </v-row>

      <v-row justify="center">
        <v-col v-for="k in 2" :key="k" cols="4">
          <v-sheet class="pa-2 ma-2"> .justify-center </v-sheet>
        </v-col>
      </v-row>

      <v-row justify="end">
        <v-col v-for="k in 2" :key="k" cols="4">
          <v-sheet class="pa-2 ma-2"> .justify-end </v-sheet>
        </v-col>
      </v-row>

      <v-row justify="space-around">
        <v-col v-for="k in 2" :key="k" cols="4">
          <v-sheet class="pa-2 ma-2"> .justify-space-around </v-sheet>
        </v-col>
      </v-row>

      <v-row justify="space-between">
        <v-col v-for="k in 2" :key="k" cols="4">
          <v-sheet class="pa-2 ma-2"> .justify-space-between </v-sheet>
        </v-col>
      </v-row>
    </v-container>
    <div class="text-center">
      <v-rating
        v-model="rating"
        bg-color="orange-lighten-1"
        color="blue"
      ></v-rating>
    </div>
    <v-main>
      <Form />
    </v-main>
  </v-app>
</template>

<style scoped>
.v-main {
  padding: 1rem 0;
  background: Green;
}
</style>
