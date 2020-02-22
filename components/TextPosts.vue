<template lang="html">
  <div class="text-box">
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article btn-4 how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article btn-4 how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>
    <div class="article btn-4">
      <h3>Flash your Radeon BIOS</h3>
      <p>Small article btn-4 how to flash your Radeon 5600XT videocard BIOS</p>
      <a href="#"></a>
    </div>

    <div class="article btn-4">
      test1
    </div>
    <div class="article btn-4">
      test2
    </div>
    <div class="article btn-4">
      test4
    </div>
    <div class="article btn-4">
      test
    </div>
    <div class="article btn-4">
      test1
    </div>
    <div class="article btn-4">
      test2
    </div>
    <div class="article">
      test4
    </div>

    <div class="article">
      test1
    </div>
    <div class="article">
      test2
    </div>
    <div class="article">
      test4
    </div>
    <div class="article">
      test
    </div>
    <div class="article">
      test1
    </div>
    <div class="article">
      test2
    </div>
    <div class="article">
      test4
    </div>

  </div>
</template>

<script>
// import OtherComponent from './OtherComponent.vue'
export default {
  name: 'TextPosts',
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

<style lang="scss" scoped>
// *{
//   outline: 1px solid magenta;
// }
$menubuttons:#333333;
$menubuttonsactive:#000000;
$menubuttonsborder:$menubuttonsactive;
$bg:#333333;
$light-bg:#ffffff;
$dark-bg:#dddddd;
$randomNumber1: random(255);
$randomNumber2: random(255);
$randomNumber3: random(255);
$randomNumber: '-'+$randomNumber1+'-'+$randomNumber2+'-'+$randomNumber3;
.text-box{
  // top:300px;
  background-color: $bg;
  // width: 100%;
  display: grid;
  grid-gap:1em;
  padding:1em;
  grid-auto-rows:1fr;
  grid-template-columns: repeat(3, 1fr);
  // padding: 0px 20px 0px 20px;
  /* grid-template-columns: 20% 20% 20% 20% 20%; */
  font-size: 25px;
}
.text-box > div.article{
  background-color: $light-bg;
  padding: 1em;
}
.text-box > div.article:nth-child(odd){
  background-color: $dark-bg;
  padding: 1em;
}
.article{
  margin: 0px;
  padding: 10px 10px 10px 10px;
  h3{
    margin: 20px 0px 0px 0px;
    font-family: 'Courier New', Courier, monospace;
    font-size: 32px;
    text-align: center;
  }
  p{
    margin: 20px 0px 20px 0px;
    font-family: 'Courier New', Courier, monospace;
    font-size: 16px;
    text-align: justify;
    text-justify: inter-character;
  }
  a{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 22px;
    float: right;
    font-weight:bolder;
    text-align: right;
    text-decoration: none;
    text-transform: uppercase;
  }
  a::before{
    content:'read more';
    color: $bg;
  }
}
.btn-4 {
  overflow: hidden;
  position: relative;

  // span {
  //   // z-index: 20;
  // }

  &:after {
    background: $menubuttonsactive;
    content: "";
    height: 590px;
    width: 150px;
    left: -350px;
    opacity: .2;
    position: absolute;
    top: -100px;
    transform: rotate(35deg);
    transition: all 1700ms cubic-bezier(0.19, 1, 0.22, 1);
    background-color: rgb($randomNumber1,$randomNumber2,$randomNumber3);

    // z-index: -10;
  }
}
.btn-4:hover {

  &:after {
    left: 150%;
    transition: all 1700ms cubic-bezier(0.19, 1, 0.22, 1);
  }
}

</style>
