<template>
  <v-container>
    <v-row justify="center" align="center">
      <v-col cols="12">
        <img src="~assets/images/home-wood1.jpeg" width="100%" height="auto" />
      </v-col>
    </v-row>
    <v-row justify="center" align="center">
      <v-col cols="12">
        <div
          class="text-center pa-8 mb-8"
          style="background-color: #27cfb1 !important"
        >
          <h1 class="pa-2 white--text">Magic!</h1>
          <h3 class="font-weight-thin pa-4">
            Lighten the world with semasa, nature will do magic for you!
          </h3>
        </div>
      </v-col>
    </v-row>
    <v-parallax dark :src="require('@/assets/images/home-wood2.jpeg')">
      <v-row align="center" justify="center">
        <v-col class="text-center" cols="12">
          <h1 class="text-h4 font-weight-thin mb-4">Semasa Living</h1>
          <h4 class="subheading">Live with natures</h4>
        </v-col>
      </v-row>
    </v-parallax>
    <v-row justify="center" align="center">
      <v-col cols="12">
        <div class="text-center pa-8 my-8" style="background-color: #f3f3f3">
          <h1 class="pa-2" style="color: #27cfb1">Natures!</h1>
          <h3 class="font-weight-thin pa-4">
            Free your mind with natures power.
          </h3>
        </div>
      </v-col>
    </v-row>
    <v-parallax dark :src="require('@/assets/images/home-wood3.jpeg')">
    </v-parallax>
    <v-row justify="center" align="center">
      <v-col cols="12">
        <div
          class="text-center pa-8 my-8"
          style="background-color: black; color: #27cfb1"
        >
          <h1 class="pa-2">Choose</h1>
          <h3 class="font-weight-normal pa-4">
            Every people have the freedom to choose.
          </h3>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
