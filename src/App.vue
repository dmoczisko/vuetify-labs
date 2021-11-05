<template>
  <v-app>
    <v-app-bar
      app
      color="#563270"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Hogwarts Logo"
          class="shrink mr-2"
          contain
          src="./assets/hogwarts.png"
          transition="scale-transition"
          width="60"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="#"
        target="_blank"
        text
      >
        <span class="mr-2">Hogwarts History</span>
        <v-icon>mdi-magic-staff</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <vuetify-tables/>
    </v-main>
  </v-app>
</template>

<script>
import VuetifyTables from './components/VuetifyTables';

export default {
  firstName: 'App',

  components: {
    // HelloWorld,
    VuetifyTables,
  },

  data: () => ({
    //
  }),
};
</script>

<style>

.hogwartsTable {
  margin-top: 20px;
}

.hogwartsTable thead span {
  font-size: 16px !important;
}

.hogwartsTable th {
  vertical-align: top;
  box-shadow: inset 0 -1px 0 rgb(86 50 112 / 100%) !important;
}



</style>