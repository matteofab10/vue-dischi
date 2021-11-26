<template>
  <header>
    <div class="logo-spotify">  
      <img src="../assets/spotify-logo.png" alt="logo-spotify">
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  header {
    height: 60px;
    background-color: #2e3a46;
    .logo-spotify {
      width: 50px;
      height: 50px;
    }
    img {
      width: 100%;
      margin: 5px 0 5px 15px;
      cursor: pointer;
    }
  
  }
  

</style>