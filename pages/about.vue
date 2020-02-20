<template lang="html">
  <div class="about">
    <Navbar/>
    <h1>About page</h1>
    <p>Some info</p>
    <Footer/>
  </div>
</template>

<script>
// import OtherComponent from './OtherComponent.vue'
import Navbar from '~/components/Navbar.vue'

import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    Footer
  }
};

</script>

<style lang="scss" scoped>
  .about{
    display:grid;
    background-color: green;
    font-size: 25px;
  }
</style>
