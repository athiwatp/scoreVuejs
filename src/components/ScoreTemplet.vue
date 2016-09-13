<template lang="html">

  <div class="container">
    <div class="row">
      <div class="col-xs-6 home">
        <span style="font-size: 120px; color: rgb(123,228,58);">{{ showData[0].title }} <br>
        {{ showData[0].score }} </span>
      </div>
      <div class="col-xs-6 away">
        <span style="font-size: 120px; color: rgb(11,63,96);"> {{ showData[1].title }} <br>
        {{ showData[1].score }} </span>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  props: ['showData']
}
</script>

<style lang="css">
  .home {
    text-align: center;
  }
  .away {
    text-align: center;
  }
  .vs {
    text-align: center;
  }
</style>
