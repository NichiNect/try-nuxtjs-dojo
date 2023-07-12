<style scoped>
  .router-link-exact-active {
    color: #eb2f9a;
  }
</style>

<template>
  <div>
    <!-- Header -->
    <header>
      <nav>
          <NuxtLink to="/">Nuxt Dojo Merch</NuxtLink>
      </nav>
    </header>

    <!-- Content -->
    <div>
      <slot />
    </div>

    <footer>
        <ul>
            <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products">Products</NuxtLink>
          </li>
        </ul>
    </footer>
  </div>
</template>