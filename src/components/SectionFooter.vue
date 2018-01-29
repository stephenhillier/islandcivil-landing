<template>
  <v-container grid-list-md text-xs-center>
    <v-divider class="footer-divider"></v-divider>
    <v-layout row wrap class="footer-text">
      <v-flex xs12 sm6 md2 offset-md3 class="stacking">
        <p><a href="#earthworks">Products</a></p>
      </v-flex>
      <v-flex xs12 sm6 md2 offset-md1>
        <p><a href="mailto:steve@islandcivil.com">Contact us</a></p>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {

}
</script>

<style>
.footer-text {
  font-family: 'Raleway', sans-serif;
  color: #2c3e50;
}
.footer-divider {
  margin-bottom: 20px;
  margin-top: -20px;
}
.stacking {
  margin-bottom: -10px;
}
</style>
