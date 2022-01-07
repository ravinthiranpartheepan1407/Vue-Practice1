<template>
  <span>
  <v-navigation-drawer app v-model="drawer" dark disable-resize-watcher>
    <v-list>
      <template v-for="(item, index) in items">
        <v-list-tile :key="index">
          <v-list-tile-content>
            {{item.title}}
          </v-list-tile-content>
        </v-list-tile>
        <v-divider :key="`divider-${index}`"></v-divider>
      </template>
    </v-list>
  </v-navigation-drawer>
  <v-toolbar app color="purple dark-4" dark>
    <v-toolbar-side-icon @click="drawer = !draw"></v-toolbar-side-icon>
    <v-toolbar-title>{{appTitle}}</v-toolbar-title>
    <v-btn to="/"> Menu </v-btn>
    <v-spacer></v-spacer>
    <v-btn to="/product"> Login </v-btn>
    <v-btn to="/content"> Content </v-btn>
    &nbsp;
    <v-spacer></v-spacer>
    <v-btn to="/resume">Resume</v-btn>
  </v-toolbar>
  </span>
</template>

<script>
  export default {
    name: 'AppNavigation',
    data() {
      return{
        appTitle: 'Meal Apps',
        items: [
          { title: 'Menu'},
          { title: 'Sign In' },
          { title: 'Join' }
        ]
      };
    }
  };
</script>

<style scoped>
</style>
