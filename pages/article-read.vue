<template lang="html">
  <div class="about">
    <Navbar/>
    <div>
      <h1> {{this.id}} </h1>
    </div>
    <Footer/>
  </div>
</template>

<script>
// import OtherComponent from './OtherComponent.vue'
import Navbar from '~/components/Navbar.vue'
import ReadPost from '~/components/ReadPost.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    ReadPost,
    Footer
  },
  data () {
    return {
      id: this.$route.params.id,
      articles: [{
        "id":"0",
        "title": "This is Title 1",
        "preview": "Small article how to flash your Radeon 5600XT videocard BIOS",
        "paragraph": [
          "Small 1 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 2 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 3 article how to flash your Radeon 5600XT videocard BIOS"
        ]
      },
      {
        "id":"1",
        "title": "This is Title 2",
        "preview": "Small article how to flash your Radeon 5600XT videocard BIOS",
        "paragraph": [
          "Small 1 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 2 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 3 article how to flash your Radeon 5600XT videocard BIOS"
        ]
      },
      {
        "id":"2",
        "title": "This is Title 3",
        "preview": "Small article how to flash your Radeon 5600XT videocard BIOS",
        "paragraph": [
          "Small 1 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 2 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 3 article how to flash your Radeon 5600XT videocard BIOS"
        ]
      },
      {
        "id":"3",
        "title": "This is Title 3",
        "preview": "Small article how to flash your Radeon 5600XT videocard BIOS",
        "paragraph": [
          "Small 1 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 2 article how to flash your Radeon 5600XT videocard BIOS",
          "Small 3 article how to flash your Radeon 5600XT videocard BIOS"
        ]
      }
    ]
    }
  },
  created(){
    this.$http.get('http://jasonplaceholder.typicode.com/posts/'+this.id).then(function(data){
      console.log(data)
    })
  }
};

</script>

<style lang="scss" scoped>
  .about{
    display:grid;
    grid-gap:3em;
    background-color: whitesmoke;
    font-size: 25px;
  }
  h1, p{
    margin: 0px 3em 0px 3em;
  }
</style>
