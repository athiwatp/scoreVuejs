<template lang="html">
  <div class="score">
    HOME <br>
    <span class="title"> {{ scoreHome }} </span>
  </div>
</template>

<script>
export default {
  props: ['scoreHome']
}
</script>

<style lang="css" scoped>
  .score {
    /*border: 8px solid #333;*/
    text-align: center;
    border-radius: 7px;
    color: green;
  }
  .title {
    text-align: center;
    font-weight: bold;
    font-size: 190px;
  }
  .scoreTemp {
    text-align: center;
  }
   .button {
     border: 8px solid #333;
     display: inline-block;
     padding-left: 2px;
     padding-right: 2px;
     text-align: center;
   }
</style>
