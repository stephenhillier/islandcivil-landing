<template>
  <v-parallax :src="getImgUrl('dam3.jpg')" height=400>
    <v-layout
      column
      align-center
      justify-center
      class="white--text"
    >
      <div class="subheading mb-1 hero-text-sub text-xs-center">Civil | Geotechnical | Mining</div>
      <p class="white--text hero-text-header mb-2 display-2 text-xs-center">Unlock the power of your knowledge</p>
      <div class="subheading mb-3 hero-text-sub text-xs-center">Find out how ISLAND Civil can help you win more contracts and deliver better solutions for your clients</div>
      <v-btn
        class="mt-5 green darken-1" dark
        primary
      >
        Learn More
      </v-btn>
    </v-layout>
  </v-parallax>
</template>

<script>
export default {
  methods: {
    getImgUrl (img) {
      return require('@/assets/' + img)
    }
  }
}
</script>

<style>
.hero-text-header {
  font-family: 'Zilla Slab', serif;
}
.hero-text-sub {
  font-family: 'Raleway', sans-serif;
}
</style>
