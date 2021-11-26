<template>
  <div class="album-box">
    <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="bon-jovi">
    <h2>new jersey</h2>
    <h4>Bon Jovi</h4>
    <h4>1988</h4>
  </div>
</template>

<script>
export default {
  name: 'Album',
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
  h4 {
    font-size: 15px;
    font-weight: 500;
    color: grey;
  }
}

</style>