<style scoped>
  h2 {
    margin-bottom: 20px;
    font-size: 36px;
  }
  p {
    margin: 20px 0;
  }
</style>

<script setup>
import ProductCard from '../../components/ProductCard.vue';

  definePageMeta({
    layout: "products",
  })

  useHead({
    title: 'Nuxt Dojo - Merch'
  })

  // * fetch API list products
  const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<template>
  <div>
    <h2>Products</h2>
    <div class="grid grid-cols-4 gap-4">
      <div v-for="item in products">
        <ProductCard :product="item" />
      </div>
    </div>
  </div>
</template>