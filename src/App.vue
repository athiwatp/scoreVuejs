<template lang="html">
  <div class="container">
      <!-- <div style="text-align:center;">Score Vuejs</div> -->
    <div class="row">
      <div class="col-md-5">
        <score-templet1 v-bind:score-home="scoreHome"></score-templet1>
      </div>
      <div class="col-md-2">
        <div class="vs"> VS </div>
      </div>
      <div class="col-md-5">
        <score-templet2 :score-away="scoreAway"></score-templet2>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6 box-content">
        <score1 :add-score-home="addScoreHome" :sub-score-home="subScoreHome"></score1>
      </div>
      <div class="col-md-6 box-content">
        <score2 :add-score-away="addScoreAway" :sub-score-away="subScoreAway"></score2>
      </div>
    </div>
  </div>
</template>

<script>
import ScoreTemplet1 from './components/ScoreTemplet1'
import Score1 from './components/score1'
import ScoreTemplet2 from './components/ScoreTemplet2'
import Score2 from './components/score2'
export default {
  data () {
    return {
      scoreHome: 0,
      scoreAway: 0
    }
  },
  computed: {},
  ready () {},
  attached () {},
  methods: {
    addScoreHome: function (score) {
      this.scoreHome += score
    },
    subScoreHome: function (score) {
      if (this.scoreHome === 0) {
        this.scoreHome = 0
      } else this.scoreHome -= score
    },
    addScoreAway: function (score) {
      this.scoreAway += score
    },
    subScoreAway: function (score) {
      if (this.scoreAway === 0) {
        this.scoreAway = 0
      } else this.scoreAway -= score
    }
  },
  components: {
    ScoreTemplet1: ScoreTemplet1,
    Score1: Score1,
    ScoreTemplet2: ScoreTemplet2,
    Score2: Score2
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
.vs {
  font-size: 137px;
padding-left: 0%;
padding-top: 44%;

}
</style>
