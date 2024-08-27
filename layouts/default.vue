<template>
    <div>
      <header class="shadow-sm bg-white">
        <nav class="container mx-auto p-4 flex justify-between">
          <NuxtLink to="/" class="font-bold">Nuxt Dojo</NuxtLink>
          <ul class="flex gap-4">
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
            <li><NuxtLink to="/products" class="btn">products</NuxtLink></li>
       
          </ul>
        </nav>
      </header>
  
      <main class="container mx-auto p-4">
      <slot /> <!-- Page content will be injected here -->
    </main>
    </div>
  </template>
  
  <script setup>
  // Any setup code if needed
  </script>
  
  <style scoped>
  /* Styles for the layout */
  header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  ul {
    list-style-type: none;
    display: flex;
    gap: 10px;
  }
  
  .router-link-exact-active {
    color: rgb(55, 55, 250); /* Active link style */
  }
  </style>
  