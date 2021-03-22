<template>
  <div id="app">
  <ProductListOne v-bind:products="products" />
  <ProductListTwo  v-bind:products="products" />
  </div>
</template>

<script>
import ProductListOne from './components/ProductListOne'
import ProductListTwo from './components/ProductListTwo'
export default {
  name: 'App',
  components: {
    ProductListOne,
    ProductListTwo
  },
  data(){
    return{
      products: [
        {name: 'banana skin', price: 20},
        {name: 'shiny star', price: 40},
        {name: 'watermelon', price: 35},
        {name: 'red shells', price: 75},
      ]
    }
  }
}
</script>

<style>
body{
  font-family: Ubuntu;
  color: #555;
}
</style>
