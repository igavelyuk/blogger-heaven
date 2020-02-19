<template>
  <div class="container">
    <Navbar/>
    <div class="main-content">
      <div class="left-side">
        <TextPosts/>
      </div>
      <div class="right-side">
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
        <Youtube/>
      </div>
    </div>


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
*{outline:1px solid blue;}
.container {
  /* margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center; */
  background-color: black;
  /* width: 100%; */
  /* display: grid; */
  /* grid-gap:1em; */
  /* grid-auto-rows: 200px; */
  /* grid-template-columns: 100%; */
  /* padding: 0px 20px 0px 20px; */
  /* grid-template-columns: 20% 20% 20% 20% 20%; */
  font-size: 25px;
}
.main-content{
  display: grid;
  grid-gap:5em;
  /* grid-auto-rows: 200px; */
  /* grid-template-columns: 100%; */
  /* padding: 0px 20px 0px 20px; */
  grid-template-columns: 60% 40%;
}
.left-side{
  display: grid;
  justify-content: start;
  /* align-content: center; */
  margin:10px;
}
.right-side{
  display: grid;
  justify-content: start;
  /* align-content: center; */
  margin:10px;
}

</style>
