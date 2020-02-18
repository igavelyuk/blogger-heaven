<template lang="html">
  <div class="navbar">
navbar
  </div>
</template>

<script>
// import OtherComponent from './OtherComponent.vue'
export default {
  components: {
    // OtherComponent
  },
  data () {
    return {
      greeting: 'Hello'
    }
  }
}
</script>

<style lang="css" scoped>
.navbar{
  background-color: red;
  height: 200px;
  width: 100%;
}
</style>
