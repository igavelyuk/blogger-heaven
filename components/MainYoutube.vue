<template>
  <div class="">
    <Navbar/>
    <div v-bind:class="color">
      {{articlename}}
    <!-- <h1>{{this.infox}}</h1> -->
    <Youtube v-for="joke in jokes" :key="joke.id" :id="joke.id" :joke="joke.joke" class="youtube"/>

      <!-- <div class="right-side">

      </div> -->
    </div>
<!-- /////////////////////////////////////////////////////// -->


<!-- ////////////////////////////////////////////////////// -->

    <Footer/>
  </div>
</template>

<script>
import axios from 'axios'
import Youtube from '~/components/Youtube.vue'

export default {
  name: 'Main Youtube',
  props:['color','articlename'],
  components: {
    Youtube
  },
  data(){
    return{
      jokes:[]
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
  async created(){
    const config = {
      headers: {
        'Accept': 'application/json'
      }
    }
    try {
      const res = await axios.get("https://icanhazdadjoke.com/search", config)
      console.log(res.data)
      this.jokes = res.data.results
    } catch (err) {
      console.log(err)
    }
  }
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
  // background-color: $bg;
  // width: 100%;
  // display: grid;
  // grid-gap:1em;
  // padding:1em;
  grid-auto-rows:1fr;
  grid-template-columns: repeat(1,1fr);
  // padding: 0px 20px 0px 20px;
  // grid-template-columns: 98%;
  // font-size: 25px;
}
.red{
  background-color: red;
}
.yellow{
  background-color: yellow;
}
.blue{
  background-color: blue;
}
// .youtube > div.article{
//   background-color: $light-bg;
//   padding: 1em;
// }
// .youtube > div.article:nth-child(odd){
//   background-color: $dark-bg;
//   padding: 1em;
// }

</style>
