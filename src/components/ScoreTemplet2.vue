<template lang="html">
  <div class="score">
    AWAY <br>
    <span class="title"> 0 </span>
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
  .score {
    border: 8px solid #333;
    text-align: center;
    border-radius: 7px;
  }
  .title {
    text-align: center;
    font-weight: bold;
    font-size: 190px;
  }
</style>
