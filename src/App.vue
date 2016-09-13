<template lang="html">
        <score-templet :show-data="data"></score-templet>
        <score
        :score="data"
        :add-score-home="addScoreHome"
        :sub-score-home="subScoreHome"
        :add-score-away="addScoreAway"
        :sub-score-away="subScoreAway">
        </score>
</template>

<script>
import ScoreTemplet from './components/ScoreTemplet'
import Score from './components/score'
export default {
  data () {
    return {
      data: [
        {
          title: 'Home',
          score: 0
        },
        {
          title: 'AWAY',
          score: 0
        }
      ]
    }
  },
  computed: {},
  ready () {},
  attached () {},
  methods: {
    addScoreHome: function (score) {
      this.data[0].score += score
    },
    subScoreHome: function (score) {
      if (this.data[0].score === 0) {
        this.data[0].score = 0
      } else this.data[0].score -= score
    },
    addScoreAway: function (score) {
      this.data[1].score += score
    },
    subScoreAway: function (score) {
      if (this.data[1].score === 0) {
        this.data[1].score = 0
      } else this.data[1].score -= score
    }
  },
  components: {
    ScoreTemplet: ScoreTemplet,
    Score: Score
  }
}
</script>

<style lang="css">
  @import 'https://fonts.googleapis.com/css?family=Baloo+Chettan';
  body {
    font-family: 'Baloo Chettan', cursive;
    font-size: 20px;
  }
</style>
