<template>
    <div>
      <div class="border-b-2">
        <AppHeader />
      </div>
      <div class="flex">
        <div class="w-1/6">
          <AppSidebar />
        </div>
        <div class="w-5/6">
          <AppContent />
        </div>
      </div>
      <div>
        <AppFooter />
      </div>
    </div>
  </template>
    
  <script setup>
  import AppContent from "../components/layouts/AppContent.vue";
  import AppFooter from "../components/layouts/AppFooter.vue";
  import AppHeader from "../components/layouts/AppHeader.vue";
  import AppSidebar from "../components/layouts/AppSidebar.vue";
  </script>
    
  <style lang="scss" scoped>
  </style>