<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

const year = new Date().getFullYear()
</script>

<template>
  <!-- The <router-link> component is used to create links to different routes in the application -->
  <nav>
    <RouterLink class="logo" to="/">Svijet gljiva</RouterLink>

    <div class="nav-links">
      <RouterLink to="/">Početna</RouterLink>
      <RouterLink to="/about">O nama</RouterLink>
    </div>
  </nav>
  <!-- The <router-view> component will render the matched component for the given route -->
  <RouterView />

  <footer>
    <p>&copy; {{ year }} Svijet gljiva. Sva prava pridržana.</p>
  </footer>
</template>
