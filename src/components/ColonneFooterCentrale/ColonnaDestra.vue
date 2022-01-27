<template>
    <div>
    <ul>
      <h3>DC</h3>
      <li v-for="(elements, index) in sites" :key="index"><a href="#">{{ elements.text }}</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ColonnaDestra',
  data() {
    return{
      sites: [
        {
          text: "DC"
        },
        {
          text: "DC UNIVERSE INFINITE"
        },
        {
          text: "DC Kids"
        },
        {
          text: "DC Shop"
        },
        {
          text: "MAD Magazine"
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