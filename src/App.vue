<template>
  <div id="app">
    <product-list-one v-bind:procucts="products"></product-list-one>
     <product-list-two v-bind:procucts="products"></product-list-two>
  </div>
</template>

<script>
import ProductListOne from './components/ProductListOne';
import ProductListTwo from './components/ProductListTwo'
export default {
  name: 'app',
  data(){
    return{
     products: [
        {name: 'A', price: 200},
        {name: 'B', price: 100},
        {name: 'C', price: 50},
        {name: 'D', price: 10},
      ]
    }
  },
  components: {
    'product-list-one':ProductListOne,
    'product-list-two':ProductListTwo

  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
