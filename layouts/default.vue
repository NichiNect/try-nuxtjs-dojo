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
      </nav>
    </header>

    <!-- Content -->
    <div>
      <slot />
    </div>
  </div>
</template>