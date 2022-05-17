<template>
  <header class="header">
    <NuxtLink to="/">
      <TheLogo />
    </NuxtLink>
    <TheNavbar />
    <div class="flex items-center space-x-4">
      <NuxtLink to="/signin" class="py-2 px-4 text-lg font-semibold">
        Sign in
      </NuxtLink>
      <NuxtLink
        to="/signup"
        class="rounded-lg bg-rose-400 py-2 px-4 text-lg font-semibold text-white"
      >
        Sign up
      </NuxtLink>
    </div>
  </header>
</template>

<script>
import TheNavbar from './TheNavbar.vue'
export default {
  name: 'TheHeader',
  components: { TheNavbar },
}
</script>

<style scoped>
.header {
  @apply flex items-center justify-between py-6 px-4;
}
</style>
