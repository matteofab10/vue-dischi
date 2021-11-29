<template>
  <select class="selector">
    <option>metal</option>
    <option>jazz</option>
    <option>pop</option>
  </select>  
</template>

<script>

export default {
  name: "Selected",
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

  .selector{
  height: 30px;
  width: 100px;
  padding: 5px;
  margin-right: 10px;
}

</style>