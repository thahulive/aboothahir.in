<template>
  <div>
    <div class="section">
      <Banner/>
    </div>
    <div class="section">
      <About />
    </div>
    <div class="section">
      <h1>skills</h1>
    </div>
  </div>
  
</template>

<script>
import About from '@/components/About'
import Banner from '@/components/Banner'
export default {
  components: {
    About,
    Banner
  }
}
</script>
<style>
.section {
  min-height: 100vh;
}
</style>
