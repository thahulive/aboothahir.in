<template>
  <div
    class="banner-wrapper">
    <v-parallax
      :height="windowSize.height"
      src="/banner.jpg"
    >
      <v-layout
        v-resize="onResize"
        align-center
        column
        justify-center
      >
        <h1 class="display-2 font-weight-thin mb-3">Vuetify.js</h1>
        <h4 class="subheading">Build your application today!</h4>
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
</style>
