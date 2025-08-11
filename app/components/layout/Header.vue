<script setup lang="ts">
const img = useImage()
</script>

<template>
  <header class="bg-white/80 backdrop-blur-md sticky top-0 z-50">
    <nav class="container mx-auto px-6 py-4 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <NuxtImg class="h-8 w-8 text-primary" src="/logo.svg" alt="site-logo"
                 :placeholder="img(`/logo.svg`, { h: 8, f: 'png', blur: 2, q: 50 })"/>
        <h2 class="text-2xl font-bold text-primary">EduPath</h2>
      </div>
      <div class="hidden md:flex items-center gap-8">
        <a class="text-secondary hover:text-primary font-medium" href="#">Courses</a>
        <a class="text-secondary hover:text-primary font-medium" href="#">Features</a>
        <a class="text-secondary hover:text-primary font-medium" href="#">Testimonials</a>
        <a class="text-secondary hover:text-primary font-medium" href="#">About Us</a>
      </div>
      <div class="hidden md:flex items-center gap-4">
        <UButton class="button secondary">Log In</UButton>
        <UButton class="button primary">Sign Up</UButton>
      </div>
      <UButton class="md:hidden text-gray-600">
        <NuxtImg src="/img/svg/mobile-menu.svg" alt="site-logo"
                 :placeholder="img(`/media/logos/logo.svg`, { h: 10, f: 'png', blur: 2, q: 50 })"></NuxtImg>
      </UButton>
    </nav>
  </header>
</template>

<style scoped>

</style>