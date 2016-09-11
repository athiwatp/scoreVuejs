<template lang="html">
  <div class="container">
      Score Vuejs
    <div class="row">
      <div class="col-md-6">
        <score-templet1 v-bind:score-home="scoreHome"></score-templet1>
      </div>
      <div class="col-md-6">
        <!-- <score-templet2></score-templet2> -->
      </div>
    </div>
    <div class="row">
      <div class="col-md-6 box-content">
        <div class="scoreTemp">
          score! HOME <br>
          <div class="button" @click="addScoreHome(1)"> +1 </div>
          <div class="button" @click="addScoreHome(2)"> +2 </div>
          <div class="button" @click="addScoreHome(3)"> +3 </div>
          <div class="button" @click="subScoreHome(1)"> -1 </div>
        </div>
      </div>
      <div class="col-md-6">
        <!-- <score2></score2> -->
      </div>
    </div>
  </div>
</template>

<script>
import ScoreTemplet1 from './components/ScoreTemplet1'
import Score1 from './components/score1'
// import ScoreTemplet2 from './components/ScoreTemplet2'
// import Score2 from './components/score2'
export default {
  data () {
    return {
      scoreHome: 0
    }
  },
  computed: {},
  ready () {},
  attached () {},
  methods: {
    addScoreHome: function (score) {
      this.scoreHome += score
    }
  },
  components: {
    ScoreTemplet1: ScoreTemplet1,
    Score1: Score1
    // ScoreTemplet2: ScoreTemplet2,
    // Score2: Score2
  }
}
</script>

<style lang="css">
  @import 'https://fonts.googleapis.com/css?family=Baloo+Chettan';
  body {
    font-family: 'Baloo Chettan', cursive;
    font-size: 20px;
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
   .box-content {
     border: 8px solid #333;
   }
</style>
