<template>
  <v-app>
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
      <v-spacer></v-spacer>
      <ComponentCart/>
      <v-spacer></v-spacer>
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
//import TodoList from './components/TodoList.vue';
import ComponentCart from './components/ComponentCart.vue';

export default {
  name: 'App',

  components: {
    ComponentCart,
  },

  data: () => ({
    //
  }),
};
</script>
