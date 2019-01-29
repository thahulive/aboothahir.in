<template>
  <div class="about-wrapper">
    <v-container>
      <div class="heading-block text-uppercase text-xs-center py-5">
        <h3 class="subheading font-weight-regular">
          My Name Is
        </h3>
        <h1 class="display-2 font-weight-bold">
          Aboo Thahir
        </h1>
        <h2 class="title font-weight-light">
          Full stack developer, Designer
        </h2>
      </div>
      <div class="content-block">
        <v-layout 
          align-center 
          justify-space-around 
          row 
          fill-height>
          <v-flex 
            md6
            sm12
            xs12
            class="text-xs-justify px-2 mt-4">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </p>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </v-flex>
          <v-flex 
            md6
            sm12
            xs12>
            features goes here
          </v-flex>
        </v-layout>
      </div>
    </v-container>
  </div>
</template>

<script>
export default {}
</script>

<style>
.about-wrapper {
  min-height: 100vh;
  color: #ffffff;
  background-color: #ff3366;
}
.heading-block {
}
</style>
