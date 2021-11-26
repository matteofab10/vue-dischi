<template>
  <div class="main-background">
    <div class="container album-container">
        <Album />
        <Album />
        <Album />
        <Album />
        <Album />
        <Album />
        <Album />
        <Album />
        <Album />
        <Album />
    </div>
  </div>
</template>

<script>


import Album from './Album.vue';


export default {
  name: "Main",
  components: {
    Album,
  }
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  .main-background {
    height: calc(100vh - 60px);
    background-color: #1e2d3b;
    color: white;
    .album-container {
      display: flex;
      flex-wrap: wrap;
      padding-top: 40px;
    }
  }

</style>