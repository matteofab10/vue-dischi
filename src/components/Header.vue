<template>
  <header>
    <div class="logo-spotify">  
      <img src="../assets/spotify-logo.png" alt="logo-spotify">
    </div>
    <div>
      <Selected />
    </div>
  </header>
</template>

<script>

import Selected from './Selected.vue';

export default {
  name: "Header",
  components: {
    Selected,
  },
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  header {
    height: 60px;
    background-color: #2e3a46;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .logo-spotify {
      width: 50px;
      height: 50px;
    }
    img {
      width: 100%;
      margin-left: 15px;
      cursor: pointer;
    }
  
  }
  

</style>