<template>
    <div>
        <div class="margine">
            <img :src="dati.thumb">
            <h4>{{ dati.series }}</h4>
        </div>
    </div>
</template>

<script>

export default {
    name: 'comixbox',
    props: {
        dati: Object
    }
}
</script>

<style scoped lang="scss">

.margine{
  margin-right: 20px;
  
    h4{
      color: white;
      width: 100%;
    }
}

</style>