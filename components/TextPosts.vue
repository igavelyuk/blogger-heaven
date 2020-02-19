<template lang="html">
  <div class="text-box">
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
    </div>
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
    </div>
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
    </div>
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
    </div>
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
    </div>
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
    </div>
    <div class="article">
      <h3>Перепрошивка Видеокатры</h3>
      <p>в этой статье мы научимся обновлять биос для видеокарт radeon 5600xt</p>
      <a href="#"></a>
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
*{
  outline: 1px solid magenta;
}
$menubuttons:#333333;
$menubuttonsactive:#000000;
$menubuttonsborder:$menubuttonsactive;
$bg:#333333;
$light-bg:#aaaaaa;
$dark-bg:#333333;

.text-box{
  top:300px;
  background-color: $bg;
  // width: 100%;
  display: grid;
  grid-gap:1em;
  // grid-auto-rows: 200px;
  grid-template-columns: repeat(3, 1fr);
  padding: 0px 20px 0px 20px;
  /* grid-template-columns: 20% 20% 20% 20% 20%; */
  font-size: 25px;
}
.text-box > div{
  background-color: $light-bg;
  padding: 1em;
}
.text-box > div::nth-child(odd){
  background-color: $dark-bg;
  padding: 1em;
}
.article{
  margin: 0px;
  padding: 10px 10px 0px 10px;
  h3{
    margin: 0px 0px 20px 0px;
    font-family: 'Courier New', Courier, monospace;
    font-size: 32px;
    text-align: center;
  }
  p{
    margin: 0px 0px 20px 0px;
    font-family: 'Courier New', Courier, monospace;
    font-size: 16px;
    text-align: justify;
    text-justify: inter-character;
  }
  a{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 26px;
    float: right;
    text-align: right;
    text-decoration: none;
    text-transform: uppercase;
  }
  a::before{
    content:'читать';
  }
}

</style>
