<template>
  <div class="backgroundBlue">
    <div class="container">
      <FooterTop />
    </div>
  </div>
</template>

<script>
import FooterTop from './FooterSection/FooterTop.vue'


export default {
  name: 'Footer',
  components: {
    FooterTop,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/global.scss';

.container{
  display: flex;
  justify-content: center;
}

.backgroundBlue{
  background-color: blue;
  padding: 20px;
}

</style>
