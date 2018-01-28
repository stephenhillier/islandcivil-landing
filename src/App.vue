<template>
  <v-app>
    <v-toolbar app class="white">
      <v-spacer class="hidden-sm-and-up" style="margin-left: -10px"/>
      <v-toolbar-title class="brand-logo">
        ISLAND
      </v-toolbar-title>
      <v-spacer/>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn flat info v-for="item in menu" :key="item.name">{{ item.name }}</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-list class="hidden-sm-and-up">
      <v-layout column align-center justify-center>
        <v-list-tile v-for="item in menu" :key="item.name">
          <v-list-tile-content>
            <v-btn flat info>{{ item.name }}</v-btn>
          </v-list-tile-content>
        </v-list-tile>
      </v-layout>
    </v-list>
    <v-content>
      <router-view/>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      menu: [
        { name: 'Solutions' },
        { name: 'Pricing' },
        { name: 'Try a Demo' }
      ]
    }
  },
  name: 'App'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Zilla+Slab');
.brand-logo {
  font-family: 'Zilla Slab', serif;
  font-size: 48px;
  font-weight: bold;
  color: #2c3e50;
}
</style>
