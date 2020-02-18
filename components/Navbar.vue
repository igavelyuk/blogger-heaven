<template lang="html">
  <div class="navbar">
      <div class="logoitem">
        <Logo/>
      </div>
      <div class="menuitems">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Merch</a></li>
          <li><a href="#">About</a></li>
        </ul>
      </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
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
*{
  outline: 1px solid red;
}
.navbar{
  display: grid;
  background-color: lightskyblue;
  height: 200px;
  grid-template-columns: 20% 80%;
}
.logoitem{
  display: grid;
}
.menuitem{
  display: grid;
  grid-template-columns: 20% 80%;
  border: 1px solid black;
}
li{
  vertical-align: center;
  display:inline-block;
  font-size: 30px;
  font-family: sans-serif;
}


</style>
