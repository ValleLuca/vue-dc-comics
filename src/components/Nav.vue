<template>
  <div class="container_Header">
    <nav>
      <ul>
        <li v-for="(elements, index) in menu" :key="index">
          <a href="#">{{ elements.testo }}</a>
        </li>
      </ul>
    </nav>
  </div>    
</template>

<script>
export default {
  name: 'Nav',
  data() {
    return{
      menu: [
        {
          testo: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          testo: "COMICS",
          url: "#",
          current: false,
        },
        {
          testo: "MOVIES",
          url: "#",
          current: false,
        },
        {
          testo: "TV",
          url: "#",
          current: false,
        },
        {
          testo: "GAMES",
          url: "#",
          current: false,
        },
        {
          testo: "COLLECTIBLES",
          url: "#",
          current: false,
        },
        {
          testo: "VIDEO",
          url: "#",
          current: false,
        },
        {
          testo: "FANS",
          url: "#",
          current: false,
        },
        {
          testo: "NEWS",
          url: "#",
          current: false,
        },
        {
          testo: "SHOP",
          url: "#",
          current: false,
        },
      ]
    }

  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/partials/variables.scss';

ul {
  display: flex;
  list-style-type: none;
  justify-content: center;

  li{
     

     a{
       text-decoration: none;
       color: black;
       padding: 50px 20px;
       &:hover{
         color: $colorePrimario;
         border-bottom: 4px solid $colorePrimario;
       }
     }
  }

}

</style>
