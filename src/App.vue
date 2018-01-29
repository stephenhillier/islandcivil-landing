<template>
  <v-app>
    <v-toolbar app class="white">
      <v-spacer class="hidden-sm-and-up" style="margin-left: -10px"/>
      <v-toolbar-title class="text-xs-center brand-logo">
        ISLAND<span class="hidden-xs-only blue--text text--darken-3 accented-text">Civil</span>
      </v-toolbar-title>
      <v-spacer/>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn flat class="blue--text text--darken-2 accented-text" v-for="item in menu" :key="item.name">{{ item.name }}</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <hero/>
    <v-list class="hidden-sm-and-up">
      <v-layout column align-center justify-center>
        <v-list-tile v-for="item in menu" :key="item.name">
          <v-list-tile-content>
            <v-btn flat class="blue--text text--darken-2">{{ item.name }}</v-btn>
          </v-list-tile-content>
        </v-list-tile>
      </v-layout>
    </v-list>
    <painpoint/>
    <products/>
  </v-app>
</template>

<script>
import Hero from '@/components/Hero'
import Products from '@/components/SectionProducts'
import Painpoint from '@/components/SectionPainpoint'

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
  name: 'App',
  components: {
    'hero': Hero,
    'products': Products,
    'painpoint': Painpoint
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Zilla+Slab');
@import url('https://fonts.googleapis.com/css?family=Raleway');
.brand-logo {
  font-family: 'Zilla Slab', serif;
  font-size: 36px;
  font-weight: bold;
  color: #2c3e50;
  padding-bottom: 0px;
  margin-bottom: 0px;
}
.accented-text {
  font-family: 'Raleway', sans-serif;
}
</style>
