<template>
  <div class="backImage">
    <div class="backgroundBlue">
        <FooterTop />
    </div>
    <div class="container">
      <div class="colonne">
        <div>
          <ColonnaSinistra />
        </div>
        <div>
          <ColonnaCentrale />
        </div>
        <div>
          <ColonnaDestra />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import FooterTop from './FooterSection/FooterTop.vue'
import ColonnaSinistra from './ColonneFooterCentrale/ColonnaSinistra.vue'
import ColonnaCentrale from './ColonneFooterCentrale/ColonnaCentrale.vue'
import ColonnaDestra from './ColonneFooterCentrale/ColonnaDestra.vue'


export default {
  name: 'Footer',
  components: {
    FooterTop,
    ColonnaSinistra,
    ColonnaCentrale,
    ColonnaDestra,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/global.scss';

.backImage{
  background-image: url("../assets/img/footer-bg.jpg");
}

.backgroundBlue{
  background-color: blue;
  padding: 20px;
  display: flex;
  justify-content: center;
}

.colonne{
  display: flex;
  padding: 20px;
    div{
      margin-right: 20px;
    }
}

</style>
