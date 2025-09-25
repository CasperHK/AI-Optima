<template>
  <nav class="top-nav" role="navigation" aria-label="Main navigation">
    <div class="container">
      <div class="brand">
        <NuxtLink to="/" class="logo">AI Optima</NuxtLink>
      </div>
      <ul class="links">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/benchmarks">Benchmarks</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/contact">Contact</NuxtLink></li>
      </ul>
    </div>
  </nav>
</template>

<script setup lang="ts">
// Pure presentational component for the top navigation
</script>

<style scoped>
.top-nav {
  position: sticky;
  top: 0;
  z-index: 1000;
  width: 100%;
  background: #0f172a; /* deep slate */
  color: #fff;
  box-shadow: 0 2px 8px rgba(2,6,23,0.12);
}
.top-nav .container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0.6rem 1.5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.logo {
  color: #fff;
  font-weight: 700;
  text-decoration: none;
  font-size: 1.15rem;
}
.links {
  display: flex;
  gap: 1.25rem;
  list-style: none;
  margin: 0;
  padding: 0;
}
.links a {
  color: rgba(255,255,255,0.9);
  text-decoration: none;
  font-weight: 600;
}
.links a:hover {
  color: #7dd3fc; /* sky-300 */
}

@media (max-width: 720px) {
  .links { display: none; }
}
</style>
