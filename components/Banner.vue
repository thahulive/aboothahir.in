<template>
  <div
    class="banner-wrapper">
    <v-parallax
      :height="windowSize.height"
      src="/banner.jpg"
    >
      <v-layout
        v-resize="onResize"
        align-start
        row
        justify-center
      >
        <div 
          class="heading-block text-uppercase text-xs-center pt-3 white--text">
          <h3 
            class="subheading font-weight-regular text-bg" 
            color="white"
            style="padding: 15px 2rem 0">
            My Name Is
          </h3>
          <h1 
            class="display-3 font-weight-bold text-bg"
            style="padding: 0 2rem;">
            Aboo Thahir
          </h1>
          <h2 
            class="title font-weight-light text-bg"
            style="padding: 0 2rem 15px">
            Full stack developer, Designer
          </h2>
        </div>
      </v-layout>
      <v-layout
        v-resize="onResize"
        align-end
        row
        justify-end
      >
        <div 
          class="text-xs-center blue-grey--text" 
          style="margin-bottom: 1% !important;">
          <h2 class="title font-weight-light">
            <v-icon color="red">info</v-icon> This site is under construction
          </h2>
        </div>
      </v-layout>
    </v-parallax>
  </div>
</template>

<script>
export default {
  data() {
    return {
      windowSize: {
        width: 0,
        height: 700
      }
    }
  },
  mounted() {
    this.onResize()
  },
  methods: {
    onResize() {
      this.windowSize = { width: window.innerWidth, height: window.innerHeight }
    }
  }
}
</script>

<style>
.banner-wrapper {
  background-color: #c9e1dd;
}
.text-bg {
  background: #1ad2c7;
  box-decoration-break: clone;
}
</style>
