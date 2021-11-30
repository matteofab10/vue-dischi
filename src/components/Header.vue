<template>
  <header>
    <div class="logo-spotify">  
      <img src="../assets/spotify-logo.png" alt="logo-spotify">
    </div>

    <select class="selection" v-model="genre" @change="$emit('changeGenre', genre)">
      <option value="" selected>Seleziona il tuo genere</option>
      <option value="Jazz">Jazz</option>
      <option value="Pop">Pop</option>
      <option value="Metal">Metal</option>
      <option value="Rock">Rock</option>
    </select>
  </header>
</template>

<script>

export default {
  name: "Header",
  props: {

  },
  data(){
    return {
      genre: ''
    }
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
    .selection{
      height: 30px;
      margin-right: 15px;
    }
  }
  

</style>