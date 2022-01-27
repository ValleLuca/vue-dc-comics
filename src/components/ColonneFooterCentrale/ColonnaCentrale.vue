<template>
  <div>
    <ul>
      <h3>DC</h3>
      <li v-for="(elements, index) in dc" :key="index"><a href="#">{{ elements.text }}</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ColonnaCentrale',
  data() {
    return{
      dc: [
        {
          text: "Terms of Use"
        },
        {
          text: "Privacy Policy (New)"
        },
        {
          text: "Ad Choices"
        },
        {
          text: "Advertising"
        },
        {
          text: "Jobs"
        },
        {
          text: "Subscriptions"
        },
        {
          text: "Talens Workshops"
        },
        {
          text: "CPSC Certificates"
        },
        {
          text: "Ratings"
        },
        {
          text: "Shop Help"
        },
        {
          text: "Contact Us"
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