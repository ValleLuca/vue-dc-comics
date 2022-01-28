<template>
    <div class="dBox" >
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

.dBox{
    width: 16%;
    padding: 20px;
    .margine{
    margin-right: 20px;
    
        h4{
        color: white;
        width: 100%;
        }
    }
}


</style>