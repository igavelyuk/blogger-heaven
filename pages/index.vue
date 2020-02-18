<template>
  <div class="container">
    <Navbar/>
    <TextPosts/>
    <Youtube/>
    <Footer/>
  </div>
</template>

<script>

import Navbar from '~/components/Navbar.vue'
import TextPosts from '~/components/TextPosts.vue'
import Youtube from '~/components/Youtube.vue'

export default {
  components: {
    Navbar,
    TextPosts,
    Youtube
  }
}
</script>

<style>
.container {
  /* margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center; */
}

</style>
