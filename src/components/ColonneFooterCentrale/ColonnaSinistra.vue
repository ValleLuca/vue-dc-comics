<template>
  <div>
    <ul>
      <h3>DC COMICS</h3>
      <li v-for="(elements, index) in dccomics" :key="index"><a href="#">{{ elements.testo }}</a></li>
    </ul>
    <ul>
      <h3>SHOP</h3>
      <li v-for="(elements, index) in shop" :key="index"><a href="#">{{ elements.text }}</a></li>
    </ul>
  </div>
    
</template>

<script>
export default {
  name: 'ColonnaSinistra',
  data() {
    return{
      dccomics: [
        {
          testo: "Characters",
        },
        {
          testo: "Comics",
        },
        {
          testo: "Movies",
        },
        {
          testo: "Tv",
        },
        {
          testo: "Games",
        },
        {
          testo: "Collections",
        },
        {
          testo: "Video",
        },
        {
          testo: "Fans",
        },
        {
          testo: "News",
        },
        {
          testo: "Shop",
        },
      ],
      shop: [
        {
          text: "Shop Dc"
        },
        {
          text: "Shop DC Collectibles"
        },
      ]
    }

  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';

ul {
  h3{
    color: $coloreSecondario;
  }

  li{
    list-style-type: none;
    
    a{
      color: $coloreFooter;
      text-decoration: none;
      &:hover{
        color: $colorePrimario;
      }
    }
  }

}


</style>
