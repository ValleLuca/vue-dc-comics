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
    <div class="lastFooter">
      <div class="container containerFooter">
        <div>
          <div class="sign">SIGN-UP NOW!</div>
        </div>
        <div class="dFlexIcons">
          <h3>FOLLOW US</h3>
          <div v-for="(elements, index) in icons" :key="index" class="pIcons">
            <img :src="elements.icone">
          </div>
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
  data() {
    return{
      icons: [
        {
          icone: require("../assets/img/footer-facebook.png")
        },
        {
          icone: require("../assets/img/footer-periscope.png")
        },
        {
          icone: require("../assets/img/footer-pinterest.png")
        },
        {
          icone: require("../assets/img/footer-twitter.png")
        },
        {
          icone: require("../assets/img/footer-youtube.png")
        },
      ]
    }

  },
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

.lastFooter{
  background-color: black;
}

.sign{
  border: 1px blue solid;
  color: white;
  padding: 10px;
}

.containerFooter{
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 30px;
}

h3{
  color: blue;
}

.dFlexIcons{
  display: flex;
}

.pIcons{
  margin-left: 10px;
}

</style>
