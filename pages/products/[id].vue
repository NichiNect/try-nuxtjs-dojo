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
import ProductDetail from '../../components/ProductDetail.vue';

	const { id } = useRoute().params

  definePageMeta({
    layout: "products"
  })

  // * fetch API single product by id
  const { data: product } = await useFetch(`https://fakestoreapi.com/products/${id}`, { key: id })

  if (!product.value) {
    throw createError({
      statusCode: 404,
      statusMessage: 'Product not found',
      fatal: true
    })
  }
</script>

<template>
  <div>
    <ProductDetail :product="product" />
  </div>
</template>