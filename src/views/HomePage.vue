<template>
  <div>
    <h1>Product List</h1>
    <div v-for="product in products" :key="product.name">
      <h2>BaoBQ</h2>
      <h3>{{ product.name }}</h3>
      <p>Price: {{ product.price }}</p>
      <p>Count: {{ product.count }}</p>
    </div>
    <router-link to="/">Go to Home</router-link>
    <router-link to="/about">Go to About</router-link>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  data() {
    return {
      products: [
        { name: 'Product A', price: 100, count: 3 },
        { name: 'Product B', price: 200, count: 3 },
        { name: 'Product C', price: 300, count: 3 }
      ]
    }
  }
}
</script>

<style scoped>

</style>
