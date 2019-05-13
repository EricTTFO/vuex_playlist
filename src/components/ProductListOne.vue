<template>
  <div id="Product-list-one">
    <h2>Product-list-one</h2>
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

<style>

</style>
