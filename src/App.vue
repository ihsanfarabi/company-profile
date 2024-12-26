<!-- src/App.vue -->
<template>
  <div id="app">
    <!-- Header / Navbar (optional) -->
    <header>
      <nav class="navbar">
        <router-link to="/">Home</router-link>
      </nav>
    </header>

    <!-- Main Content Area -->
    <main>
      <!-- Renders the active route’s component -->
      <router-view />
    </main>

    <!-- Footer -->
    <footer class="footer">
      <p>&copy; {{ currentYear }} Your Company. All rights reserved.</p>
    </footer>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

// Get the current year (just a small example of using composition API here)
const currentYear = ref(new Date().getFullYear());
</script>
