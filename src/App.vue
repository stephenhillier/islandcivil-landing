<template>
  <v-app>
    <v-toolbar app class="white">
      <v-spacer class="hidden-sm-and-up brand-spacer"/>
      <v-toolbar-title class="text-xs-center brand-logo">
        <v-icon x-large class="primary--text hidden-sm-and-down brand-icon">filter_hdr</v-icon>ISLAND<span class="blue--text text--darken-3 accented-text">Civil</span>
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
    <demo/>
    <consulting/>
    <ic-footer/>
  </v-app>
</template>

<script>
import Hero from '@/components/Hero'
import Products from '@/components/SectionProducts'
import Painpoint from '@/components/SectionPainpoint'
import Consulting from '@/components/SectionConsulting'
import Demo from '@/components/SectionDemo'
import Footer from '@/components/SectionFooter'

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
    'painpoint': Painpoint,
    'consulting': Consulting,
    'demo': Demo,
    'ic-footer': Footer
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
}
.brand-spacer {
  margin-left: -10px!important;
}
.brand-icon {
  margin-top: -3px;
}
.accented-text {
  font-family: 'Raleway', sans-serif;
}
.product-title {
  font-family: 'Raleway', sans-serif;
  font-weight: bold;
  color: #2c3e50;
}
p {
  font-family: 'Raleway', sans-serif;
}
</style>
