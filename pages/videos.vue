<template>
  <div class="container">
    <Navbar/>
    <div class="youtube">
    <!-- <h1>{{this.infox}}</h1> -->
      <div class="red">
          <MainYoutube color="red" articlename="Computers"/>
      </div>
      <div class="yellow">
          <MainYoutube color="yellow" articlename="DIY"/>
      </div>
      <div class="blue">
          <MainYoutube color="blue" articlename="Programming"/>
      </div>
    </div>
<!-- /////////////////////////////////////////////////////// -->


<!-- ////////////////////////////////////////////////////// -->

    <Footer/>
  </div>
</template>

<script>
import axios from 'axios'
import Navbar from '~/components/Navbar.vue'
import Youtube from '~/components/Youtube.vue'
import Footer from '~/components/Footer.vue'
import MainYoutube from '~/components/MainYoutube.vue'

export default {
  name: 'VideosPage',
  components: {
    Navbar,
    Youtube,
    MainYoutube,
    Footer
  },
  data(){
    return{
      // videos:[]
    }
  },
  // filters:{
  //
  // },
  // mounted:{
  //
  // },
  // methods:{
  //
  // },
  // computed:{
  //
  // },
  // updated:{
  //
  // },
  // async created(){
  //   const config = {
  //     headers: {
  //       'Accept': 'application/json'
  //     }
  //   }
  //   try {
  //     const res = await axios.get("https://icanhazdadjoke.com/search", config)
  //     console.log(res.data)
  //     this.jokes = res.data.results
  //   } catch (err) {
  //     console.log(err)
  //   }
  // }
  // finish export
}
</script>

<style lang="scss" scoped>
// *{outline:1px solid blue;}
$bg: #333555;
$light-bg: #333555;
$dark-bg: #333555;
.youtube{
  // top:300px;
  background-color: $bg;
  // width: 100%;
  display: grid;
  // grid-gap:1em;
  // padding:1em;
  grid-auto-rows:1fr;
  grid-template-columns: repeat(3, 1fr);
  // padding: 0px 20px 0px 20px;
  /* grid-template-columns: 20% 20% 20% 20% 20%; */
  font-size: 25px;
}
.youtube > div.article{
  background-color: $light-bg;
  padding: 1em;
}
.youtube > div.article:nth-child(odd){
  background-color: $dark-bg;
  padding: 1em;
}

</style>
