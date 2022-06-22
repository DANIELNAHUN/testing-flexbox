<template>
  <v-app style="background : #0A0C1B">
    <v-app-bar
      app
      color="purple"
      dark
      clipped-left
    >
    <v-spacer></v-spacer>
    <h3 class="text-center">MI PRIMER PROYECTO</h3>
    <v-spacer></v-spacer>
      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-umbrella-closed</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <v-container>
        <div class="d-flex justify-center py-3"><ComponentCart/></div>
        <div class="d-flex justify-center py-3"><CardBusiness/></div>
        <div class="d-flex justify-center py-3"><ThreeCards/></div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
//import TodoList from './components/TodoList.vue';
import CardBusiness from './components/CardBusiness.vue';
import ComponentCart from './components/ComponentCart.vue';
import ThreeCards from './components/ThreeCards.vue';

export default {
  name: 'App',

  components: {
    CardBusiness,
    ComponentCart,
    ThreeCards,
  },

  data: () => ({
    //
  }),
};
</script>
