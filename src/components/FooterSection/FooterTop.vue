<template>
  <div class="boxDC">
    <div v-for="(elements, index) in box" :key="index" class="paddingBox">
      <img :src="elements.image">
      <span>{{ elements.text }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterTop',
  data() {
    return{
      box: [
        {
          image: "../../assets/img/buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          image: "../../assets/img/buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          image: "../../assets/img/buy-comics-shop-locator.png",
          text: "SUBSCRIPTION",
        },
        {
          image: "../../assets/img/buy-comics-subscriptions.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          image: "../../assets/img/buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ]
    }

  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.boxDC{
  display: flex;
}

.paddingBox{
  padding: 20px;
}

</style>