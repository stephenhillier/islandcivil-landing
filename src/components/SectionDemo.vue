<template>
  <v-container grid-list-md mt-2>
    <v-divider class="mb-5"/>
    <v-layout row wrap>
      <v-flex xs12 sm6 md4 offset-md1>
        <h3 class="display-1 product-title mt-3">Earthworks Features</h3>
        <p class="mt-5 demo-text primary--text"><v-icon left class="blue--text text--darken-2" style="margin-top: -5px;">thumb_up</v-icon> Easy to use</p>
        <p>We know it's tough to get people trained on new software, so we made sure the Earthworks line of products are intuitive and easy to use.</p>

        <p class="mt-5 demo-text primary--text"><v-icon left class="blue--text text--darken-2" style="margin-top: -5px;">build</v-icon> Tailored for you</p>
        <p>Every organization is different. We'll work with you to make sure you get a product that meets your needs. If something is missing, we'll build it!</p>

        <p class="mt-5 demo-text primary--text"><v-icon left class="blue--text text--darken-2" style="margin-top: -5px;">trending_up</v-icon> Makes you look good</p>
        <p>Earthworks products help you deliver more professional borehole logs and lab reports.</p><p>Input is checked against standard classifications (USCS) and your own guidelines to ensure a consistent style.</p>

        <v-divider class="hidden-sm-and-up"></v-divider>
      </v-flex>
      <v-flex xs12 sm6 md5 offset-md1>
        <v-card class="blue" dark>
          <v-card-text>
            <v-card>
            <v-card-media :src="getImgUrl('bhmap.png')" height=300></v-card-media>
            </v-card>
            </v-card-text>
            <v-card-title primary class="demo-title white--text"><v-icon x-large>pin_drop</v-icon>Visualize</v-card-title>
            <v-card-text class="demo-text">
            <p>All assets with a location are mapped. It's easy to see where your data is.</p>
            <p>Explore the map to see what's near an area of interest, or get a list of results by searching.</p>
          </v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
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
.demo-title {
  font-family: 'Raleway', sans-serif;
  font-size: 36px;
  font-weight: bold;
}
.demo-text {
  font-family: 'Raleway', sans-serif;
  font-size: 16px;
  font-weight: bold;
}
</style>
