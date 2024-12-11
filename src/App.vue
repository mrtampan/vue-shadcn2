<script setup>
import { RouterLink, RouterView } from 'vue-router';
import MainNav from './components/MainNav.vue';
</script>

<template>
  <div class="border-b">
    <div class="flex h-16 items-center px-4">
      <MainNav class="mx-6" />
    </div>
  </div>
  <RouterView />
</template>

<style scoped>

</style>
