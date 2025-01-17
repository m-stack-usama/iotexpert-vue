<script setup>
import HeaderComponent from "./HeaderComponent.vue";
import FooterComponent from "./FooterComponent.vue";
import SidebarComponent from "./SidebarComponent.vue";
</script>

<template>
  <div class="flex flex-col min-h-screen">
    <!-- Header -->
    <header class="text-white">
      <HeaderComponent />
    </header>

    <div class="flex flex-1">
      <!-- Sidebar -->
      <aside class="w-64 bg-gray-100 p-4">
        <SidebarComponent />
      </aside>

      <!-- Main Content -->
      <main class="flex-1 p-4">
        <router-view />
      </main>
    </div>

    <!-- Footer -->
    <footer class="border p-4">
      <FooterComponent />
    </footer>
  </div>
</template>
