<template lang="html">
  <div class="scoreTemp">
    score! HOME <br>
    <div class="button"> +1 </div>
    <div class="button"> +2 </div>
    <div class="button"> +3 </div>
    <div class="button"> -1 </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  computed: {},
  ready () {},
  attached () {},
  methods: {},
  components: {}
}
</script>

<style lang="css" scoped>
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
