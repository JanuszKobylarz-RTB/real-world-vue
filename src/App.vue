<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div id="layout">
    <div class="wrapper">
      <nav>
        <RouterLink :to="{ name: 'home' }">Events</RouterLink> |
        <RouterLink :to="{ name: 'about' }">About</RouterLink>
      </nav>
    </div>
    <RouterView />
  </div>
</template>

<style scoped>
#layout {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  --webkit-font-smoothing: antialiased;
  --moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
}
nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<style>
h2 {
  font-size: 20px;
}
</style>
