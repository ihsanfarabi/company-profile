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
import { ref } from 'vue'

// Get the current year (just a small example of using composition API here)
const currentYear = ref(new Date().getFullYear())

</script>

<style scoped>
/* Simple layout styling */
#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

/* Header / Navbar */
header {
  background-color: #f8f8f8;
  padding: 1rem;
}
.navbar {
  display: flex;
  gap: 1rem;
}
.navbar a {
  color: #333;
  text-decoration: none;
  font-weight: 500;
}

/* Main Content Area */
main {
  flex: 1;
  padding: 2rem;
}

/* Footer */
.footer {
  text-align: center;
  background-color: #f8f8f8;
  padding: 1rem;
  margin-top: auto;
}
</style>
