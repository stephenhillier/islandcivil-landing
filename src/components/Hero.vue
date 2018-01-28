<template>
  <v-parallax :src="getImgUrl('dam3.jpg')" height=450>
    <v-layout
      column
      align-center
      justify-center
      class="white--text"
    >
      <div class="subheading mb-1 hero-text-sub text-xs-center">Civil | Geotechnical | Mining</div>
      <p class="white--text hero-text-header mb-2 display-2 text-xs-center">Unlock the power of your engineering data</p>
      <div class="subheading mb-3 hero-text-sub text-xs-center">Find out how <span class="brand-text">ISLAND Civil</span> can help you <span class="brand-text">win more contracts</span> and <span class="brand-text">deliver better solutions</span> for your clients</div>
      <v-btn
        class="mt-3 green darken-1 accented-text" dark
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
.brand-text {
  font-weight: bold;
}
</style>
