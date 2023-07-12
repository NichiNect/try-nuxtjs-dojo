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
	const { id } = useRoute().params

  definePageMeta({
    layout: "products"
  })

  // * fetch API single product by id
  const { data: product } = await useFetch(`https://fakestoreapi.com/products/${id}`, { key: id })
</script>

<template>
  <div>
    <h2>Product Detail: {{ product.title }}</h2>
    <p>{{ product.price }}</p>
    <p>{{ product.id }}</p>
  </div>
</template>