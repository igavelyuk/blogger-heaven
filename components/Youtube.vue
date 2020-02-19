<template lang="html">
  <div class="you-box">
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>
    <div class="articlez">
      <h3>Перепрошивка Видеокатры</h3>
      <a href="#">
      <img src="https://img.youtube.com/vi/GpB7B7w2008/0.jpg" alt="">
      </a>
    </div>


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

<style lang="scss" scoped>
$light-bg:#ffffff;
$dark-bg:#dddddd;
$readmorebuttons:#333333;
.you-box{
  background-color: yellow;
  // width: 100%;
  display: grid;
  grid-template-columns: 1fr;
  // grid-auto-rows:290px;
  font-size: 25px;
}
.you-box > div.articlez{
  background-color: $dark-bg;
  padding: 1em;
}
.you-box > div.articlez:nth-child(odd){
  background-color: $readmorebuttons;
  padding: 1em;
}
.articlez{
  display: grid;
  margin: 0px;
  // padding: 10px 10px 10px 10px;
  h3{
    margin: 1px;
    font-family: 'Courier New', Courier, monospace;
    font-size: 12px;
    text-align: center;
    top:50%;
    left:50%;
  // bottom: 20px;
  // right: 20px;
    background-color: black;
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
    max-width:100%;
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
