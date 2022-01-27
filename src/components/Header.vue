<template>
  <div>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="">
      <Nav />
    </div>
    
  </div>
</template>

<script>
import Nav from './Nav.vue'

export default {
  name: 'Header',
  components: {
    Nav
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/global.scss';

.container{
  display: flex;
  align-items: center;
  justify-content: space-between;
}

</style>
