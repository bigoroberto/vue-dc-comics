<template>
  <main>
    <div class="container">
      <ProductCard 
          v-for="(product,index) in products"
          :key="index"
          :card="product"
          />
    </div>

  </main>
</template>

<script>

import products from '@/assets/data/listadc.js';
import ProductCard from "@/components/ProductCard.vue"


export default {
  name: 'MainComp',

  components:{
    ProductCard
  },
  data(){
    return{
      products
    }
  },

  mounted(){
    console.log(products)
  }
}
</script>

<style lang="scss" scoped>
main{
  padding: 50px 0;
  color: bisque;
  background-color: #1c1c1c;
  div{
    display: flex;
    flex-wrap: wrap;
  }
}

span{
  color: red
}
</style>