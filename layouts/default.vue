<style scoped>
  .router-link-exact-active {
    color: #eb2f9a;
  }
</style>

<template>
  <div>
    <!-- Header -->
    <header class="shadow-sm bg-gray-200">
      <nav class="container mx-auto p-4 flex justify-between">
        <NuxtLink to="/" class="font-bold">Nuxt Dojo</NuxtLink>
        <ul class="flex gap-4">
          <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products" class="btn">Products</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>

    <!-- Content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>
</template>