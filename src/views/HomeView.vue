<!-- src/views/HomeView.vue -->
<template>
    <section class="home-view">
      <!-- Hero Section -->
      <div class="hero">
        <h1>Welcome to Our Company</h1>
        <p>We provide world-class services to clients worldwide.</p>
      </div>
  
      <!-- Services Section -->
      <div class="services-section">
        <!-- Example of a reusable component (could be imported from '@/components/ServicesSection.vue') -->
      </div>
  
      <!-- CTA or Footer Section -->
      <div class="footer-cta">
        <p>Ready to get started or have questions?</p>
      </div>
    </section>
  </template>
  
  <style scoped>
  .home-view {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    padding: 2rem;
  }
  
  /* Hero Section */
  .hero {
    text-align: center;
    background: #f8f8f8;
    padding: 2rem;
    border-radius: 8px;
  }
  
  .hero h1 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }
  
  .hero p {
    font-size: 1.125rem;
    margin-bottom: 1rem;
  }
  
  /* Example CTA button styling */
  .cta-button {
    background-color: #007bff; /* Update to match your design */
    color: #fff;
    text-decoration: none;
    padding: 0.75rem 1.5rem;
    border-radius: 4px;
  }
  
  /* Services Section */
  .services-section {
    padding: 2rem 0;
  }
  
  /* Footer CTA */
  .footer-cta {
    text-align: center;
    background: #f0f0f0;
    padding: 1.5rem;
    border-radius: 8px;
  }
  </style>  