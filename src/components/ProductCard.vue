<template>
  <div>
    <img :src="card.thumb" :alt="series">
    <br>
   <!--  <h4>{{card.series}}</h4> -->
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props:{
    card:Object
  }
}
</script>

<style lang="scss" scoped>
div{
  display: flex;
  flex-basis: 100/6;
  img{
    padding: 7px;
    margin-bottom: 20px;
  }
}

</style>