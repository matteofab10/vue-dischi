<template>
  <div class="album-box">
    <img :src="albums.poster" :alt="albums.title">
    <h2>{{albums.title}}</h2>
    <h3>{{albums.author}}</h3>
    <h3>{{albums.year}}</h3>
  </div>
</template>

<script>
export default {
  name: 'Album',
  props:{
    albums: Object
  }
}
</script>

<style lang="scss">
@import "../assets/style/vars.scss";

.album-box {
  width: calc(100% / 5 - 40px);
  background-color: #2e3a46;
  text-align: center;
  padding: 20px;
  margin: 20px;
  padding-bottom: 70px;
  img {
    width: 100%;
    margin-bottom: 15px;
  }
  h2 {
    font-size: 20px;
    text-transform: uppercase;
    color: white;
    margin-bottom: 10px;
  }
  h3 {
    font-size: 20px;
    font-weight: 500;
    color: grey;
  }
}

</style>