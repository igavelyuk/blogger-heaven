<template lang="html">
  <div class="you-box">
    <div class="articlez">
      <h5>{{ joke }}</h5>
      <!-- <a :href="https://www.youtube.com/watch?v=r5kDCCknp4M&list=PLlpl3XXn_BinBiI04wPDAA9Vj3hPfLCwS&index=3&t=0s"> -->
      <img :src="thumb" alt="">
      <!-- </a> -->
    </div>
  </div>
</template>

<script>
// import OtherComponent from './OtherComponent.vue'
export default {
  name: 'Youtube',
  props: ['joke', 'thumb'],
  components: {
    // OtherComponent
  },
  data () {
    return {
      greeting: this.thumb
    }
  }
}
</script>

<style lang="scss" scoped>
*{outline: 1px solid green;}
$light-bg:#ffffff;
$dark-bg:#dddddd;
$readmorebuttons:#333333;
.you-box{
  background-color: rgba(100,100,100, 0.8);
  // width: 100%;
  display: grid;
  grid-template-columns: repeat(3,1fr);
  // grid-auto-rows:50%;
  font-size: 25px;
}
// .you-box > div.articlez{
//   background-color: $dark-bg;
//   padding: 1em;
// }
// .you-box > div.articlez:nth-child(odd){
//   background-color: $readmorebuttons;
//   padding: 1em;
// }
.articlez{
  // padding-top: 1em;
  display: grid;
  // grid-gap:1em;
  grid-template-columns: 1fr;
  margin: 0px;
  border: 5px solid white;
  // padding: 10px 10px 10px 10px;
}
h5{
  // float: right;
  position: relative;
  margin: 1px;
  font-family: 'Courier New', Courier, monospace;
  color:white;
  font-size: 32px;
  text-align: center;
  top:50%;

// bottom: 20px;
// right: 20px;
  background-color: rgba(10,10,10, 0.8);
  color: white;
// padding-left: 5px;
// padding-right: 5px;
}
p{
  font-family: 'Courier New', Courier, monospace;
  font-size: 16px;
  text-align: justify;
  text-justify: inter-character;
}
img{
  width:100%;
  height:auto;
  // float: left;
  // text-align: center;
}
a{
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  font-size: 22px;
  float: right;
  font-weight:bolder;
  text-align: right;
  text-decoration: none;
  text-transform: uppercase;
  color: $readmorebuttons;
}

a::before{
  content:'читать';
}
div.articlez:nth-child(even){
  a{
    color: $readmorebuttons;
  }
}
div.articlez:nth-child(odd){
  a{
    color: $light-bg;
  }
}


</style>
