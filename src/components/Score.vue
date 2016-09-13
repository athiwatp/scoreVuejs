<template lang="html">
  <div class="container">
    <div class="row">
      <div class="col-xs-6">
        <div class="button yellow" @click="addScoreHome(1)">+1</div>
        <div class="button green" @click="addScoreHome(2)">+2</div>
        <div class="button blue" @click="addScoreHome(3)">+3</div>
        <div class="button red" @click="subScoreHome(1)">-1</div>
      </div>
      <div class="col-xs-6">
        <div class="button yellow" @click="addScoreAway(1)">+1</div>
        <div class="button green" @click="addScoreAway(2)">+2</div>
        <div class="button blue" @click="addScoreAway(3)">+3</div>
        <div class="button red" @click="subScoreAway(1)">-1</div>
      </div>
    </div>
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
  components: {},
  props: ['score', 'addScoreHome', 'subScoreHome', 'addScoreAway', 'subScoreAway']
}
</script>

<style lang="css">
.button {
  display: inline-block;
  padding: 10%;
  cursor: pointer;
}
.score {
  text-align: center;
  padding-top: 0px;
}
.yellow {background-color: yellow;border-radius: 63px; font-size: 20px;}
.green {background-color: green; border-radius: 63px; font-size: 20px;}
.blue {background-color: blue; border-radius: 63px; font-size: 20px;}
.red {background-color: red; border-radius: 63px; font-size: 20px;}
</style>
