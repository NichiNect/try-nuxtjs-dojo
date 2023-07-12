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
</script>

<template>
  <div>
    <h2>Product Detail for: {{ id }}</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo ab consequatur rerum quos, reiciendis dolorum iure nobis ratione est in! Saepe nesciunt pariatur dolor nostrum neque porro fuga soluta ut!</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia quaerat quisquam laborum perspiciatis odio, eum alias impedit sint explicabo, veritatis unde laboriosam similique vel ab id aperiam cupiditate optio. Molestias?</p>
  </div>
</template>