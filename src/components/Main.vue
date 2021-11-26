<template>
  <div class="main-background">
    <div class="container album-container">
        <Album 
        v-for="(album, index) in albums"
        :key="index"
        :albums="album"/>
    </div>
  </div>
</template>

<script>

import axios from "axios";
import Album from './Album.vue';


export default {
  name: "Main",
  components: {
    Album
  },
  data(){
    return{
      albums: [],
      apiUrl: "https://flynn.boolean.careers/exercises/api/array/music"
    }
  },
  methods:{
    getApi(){
      axios.get(this.apiUrl)
        .then( r => {
          this.albums = r.data.response;
        })
        .catch( e => {
          console.log(e);
        })
    }
  },
    mounted(){
    this.getApi();
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  .main-background {
    min-height: calc(100vh - 60px);
    background-color: #1e2d3b;
    color: white;
    .album-container {
      display: flex;
      flex-wrap: wrap;
      padding-top: 50px;
    }
  }

</style>