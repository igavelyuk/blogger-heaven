<template>
  <div class="">
    <!-- <Navbar/> -->
    <div v-bind:class="color">
      {{articlename}}
    <!-- <h1>{{this.infox}}</h1> -->
    <Youtube v-for="video in videos.items" :key="video" :joke="video.snippet.title" :thumb="video.snippet.thumbnails.high.url"

     class="youtube"/>
      <!-- <div class="right-side">

      </div> -->
    </div>
    <!-- <Footer/> -->
  </div>
</template>

<script>
import axios from 'axios'
// import Navbar from '~/components/Navbar.vue'
import Youtube from '~/components/Youtube.vue'
// import Footer from '~/components/Footer.vue'

export default {
  name: 'MainYoutube',
  props:['color','articlename'],
  components: {
    // Navbar,
    Youtube,
    // Footer
  },
  data(){
    return{
      videos:[]
    }
  },
  computed: {
    reverseItems() {
      // if(this.videos.items != undefined){
        var Base = this.videos.items
        var Rev = [];
        for (var i = 0; i < Base.lenght; i++){
          Rev[Base.lenght - i] = Base.lenght[i]
        }
        this.videos.items = Rev
      // }
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
    // const config = {
      // headers: {
      //   'Accept': 'application/json'
      // },
    //   'part': 'snippet',
    //   'key': 'AIzaSyDwNbtxcWGG7CMa9byPBQbQtBhgZsb3RXM',
    //   'maxResults': '10',
    //   'playlistId': 'PLlpl3XXn_Bin98Q7fNjaTUOYQXhDZBU-i'
    // }
    try {
      const res = await axios.get("https://www.googleapis.com/youtube/v3/playlistItems?part=snippet&playlistId=PLlpl3XXn_BinBiI04wPDAA9Vj3hPfLCwS&maxResults=10&key=AIzaSyDwNbtxcWGG7CMa9byPBQbQtBhgZsb3RXM")
      console.log(res.data)
      this.videos = res.data
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
