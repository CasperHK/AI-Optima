<template>
  <TopNav />
  <main class="main-content">
    <section class="hero">
      <h1>Welcome to AI Optima</h1>
      <p>Your trusted source for AI model benchmarks and insights.</p>
      <button class="cta">Explore Benchmarks</button>
    </section>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import TopNav from '../components/TopNav.vue'

export default defineComponent({
  name: 'PagesHome',
  components: { TopNav }
})
</script>

<style scoped>
.navbar {
  position: sticky;
  top: 0;
  width: 100%;
  background: #18181b;
  color: #fff;
  z-index: 1000;
  box-shadow: 0 2px 8px rgba(0,0,0,0.04);
}
.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0.5rem 2rem;
}
.logo {
  font-size: 1.5rem;
  font-weight: bold;
  letter-spacing: 1px;
}
.nav-links {
  list-style: none;
  display: flex;
  gap: 2rem;
  margin: 0;
  padding: 0;
}
.nav-links a {
  color: #fff;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.2s;
}
.nav-links a:hover {
  color: #38bdf8;
}
.main-content {
  padding: 3rem 1rem 1rem 1rem;
  min-height: 80vh;
  background: #f4f4f5;
}
.hero {
  max-width: 700px;
  margin: 0 auto;
  text-align: center;
  padding: 4rem 2rem;
  background: #fff;
  border-radius: 1rem;
  box-shadow: 0 4px 24px rgba(0,0,0,0.06);
}
.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  color: #18181b;
}
.hero p {
  font-size: 1.25rem;
  color: #52525b;
  margin-bottom: 2rem;
}
.cta {
  background: #38bdf8;
  color: #fff;
  border: none;
  padding: 0.75rem 2rem;
  border-radius: 2rem;
  font-size: 1.1rem;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.2s;
}
.cta:hover {
  background: #0ea5e9;
}
</style>
