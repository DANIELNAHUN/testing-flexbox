<template>
  <div>
    <v-form v-model="valid">
      <v-container>
        <v-row>
          <v-col cols="12" md="4">
            <v-text-field
              v-model="todoNew.text"
              :rules="nameRules"
              :counter="10"
              label="First name"
              required
              outlined
            ></v-text-field>
            <v-btn @click="addTodoItem" color="primary"> Agregar </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </v-form>

    <v-card class="mx-auto" max-width="500">
      <v-toolbar color="pink" dark>
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>Inbox</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-checkbox-marked-circle</v-icon>
        </v-btn>
      </v-toolbar>

      <v-list two-line>
        <v-list-item-group v-model="todoSelected" active-class="pink--text">
          <template v-for="(item, index) in todoList">
            <v-list-item :key="index">
              <template v-slot:default="{ active }">
                <v-list-item-content>
                  <v-list-item-title v-text="item.text"></v-list-item-title>
                </v-list-item-content>

                <v-list-item-action>
                  <v-icon v-if="!active" color="grey lighten-1">
                    mdi-star-outline
                  </v-icon>

                  <v-icon v-else color="yellow darken-3"> mdi-star </v-icon>
                </v-list-item-action>
              </template>
            </v-list-item>

            <v-divider
              v-if="index < todoList.length - 1"
              :key="index + 'u'"
            ></v-divider>
          </template>
        </v-list-item-group>
      </v-list>
    </v-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      valid: false,
      firstname: "",
      lastname: "",
      nameRules: [
        (v) => !!v || "Name is required",
        (v) => v.length <= 10 || "Name must be less than 10 characters",
      ],
      email: "",
      emailRules: [
        (v) => !!v || "E-mail is required",
        (v) => /.+@.+/.test(v) || "E-mail must be valid",
      ],

      todoNew: {
        text: "New",
        activo: true,
        id: null,
      },

      todoList: [],
      todoSelected: null,
    };
  },
  methods: {
    addTodoItem() {
      const itemId = this.todoList.length + 1;
      const itemData = {
        text: this.todoNew.text,
        active: true,
        id: itemId,
      };

      this.todoList.push(itemData);

      console.log(this.todoList);
    },
  },
};
</script>

<style lang="scss" scoped>
</style>