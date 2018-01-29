<template>
  <v-container grid-list-md text-xs-center mt-2>
    <v-layout row wrap>
      <v-flex xs12 sm6 md4 offset-md2>
        <v-icon x-large class="info--text mt-2">cloud_queue</v-icon>
        <h3 class="display-1 product-title mt-3">Earthworks <span class="blue--text text--darken-2">Server</span></h3>
        <p class="mt-3">Earthworks Server is a powerful database server that helps your engineers and technical staff organize project data.</p>
        <p>Choose to either deploy on-site on your local network or host on a cloud provider to provide your engineers with 24/7 global access.</p>
        <v-divider class="hidden-sm-and-up"></v-divider>
      </v-flex>
      <v-flex xs12 sm6 md4>
        <v-icon x-large class="info--text mt-2">desktop_windows</v-icon>
        <h3  class="display-1 product-title mt-3">Earthworks <span class="blue--text text--darken-2">Desktop</span></h3>
        <p class="mt-3">Earthworks Desktop is a standalone desktop solution that streamlines project management and laboratory testing.</p>
        <p>Suitable for working on either a local computer or an Earthworks Server.</p>
        <v-divider class="hidden-sm-and-up"></v-divider>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {

}
</script>

<style>
.product-title {
  font-family: 'Raleway', sans-serif;
  font-weight: bold;
  color: #2c3e50;
}
p {
  font-family: 'Raleway', sans-serif;
}
</style>
