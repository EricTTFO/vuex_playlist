<template>
  <div id="Product-list-two">
    <h2>Product-list-two</h2>
    <ul>
      <li v-for="product in products>
          <span class='name'>{{ product.name }}</span>
          <span class='price'>${{ product.name }}</span>
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  props: ['products'],
  data(){
    return{
      
    }
  }
}
</script>

<style scoped>
    #Product-list-two{
        background: #D1e4ff;
        box-show: 1px 2px 3px ragb(0,0,0,0.2);
    }
</style>
