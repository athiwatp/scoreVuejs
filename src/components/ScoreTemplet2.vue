<template lang="html">
  <div class="score">
    AWAY <br>
    <span class="title"> {{scoreAway}} </span>
  </div>
</template>

<script>
export default {
  props: ['scoreAway']
}
</script>

<style lang="css" scoped>
  .score {
    /*border: 8px solid #333;*/
    text-align: center;
    border-radius: 7px;
    color: blue;
  }
  .title {
    text-align: center;
    font-weight: bold;
    font-size: 190px;
  }
</style>
