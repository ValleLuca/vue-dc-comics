<template>
  <div class="backgound">
    <div class="container">
      <div class="spanPadding">
        <span> => contenunto  </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/global.scss';

.backgound{
  background-color: black;
}

span{
  color: white;
}

.spanPadding{
  padding: 40px;
}

</style>
