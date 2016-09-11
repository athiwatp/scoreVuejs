<template lang="html">
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <score-templet1></score-templet1>
      </div>
      <div class="col-md-6">
        <score-templet2></score-templet2>
      </div>
    </div>
    <div class="row">
      <div class="col-md-6">
        <score1></score1>
      </div>
      <div class="col-md-6">
        <score2></score2>
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
    }
  },
  computed: {},
  ready () {},
  attached () {},
  methods: {},
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
</style>
