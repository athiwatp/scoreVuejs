<template lang="html">
  <div class="scoreTemp">
    score! HOME <br>
    <div class="button yellow" @click="addScoreHome(1)"> +1 </div>
    <div class="button green" @click="addScoreHome(2)"> +2 </div>
    <div class="button blue" @click="addScoreHome(3)"> +3 </div>
    <div class="button red" @click="subScoreHome(1)"> -1 </div>
  </div>
</template>

<script>
export default {
  props: ['addScoreHome', 'subScoreHome']
}
</script>

<style lang="css" scoped>
.scoreTemp {
  text-align: center;
}
 .button {
   /*border: 8px solid #333;*/
   display: inline-block;
   padding-left: 2px;
   padding-right: 2px;
   text-align: center;
   cursor: pointer;
   border-radius: 20px;
   font-size: 37px;
   width: 9%;
 }
 .yellow {
   background-color: yellow;
 }
 .green {
   background-color: green;
 }
 .blue {
   background-color: blue;
 }
 .red {
   background-color: red;
 }
</style>
