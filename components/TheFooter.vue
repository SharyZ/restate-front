<template>
  <footer class="footer">
    <div class="grid grid-cols-5">
      <div class="col-span-2">
        <TheLogo />
        <p>
          We have a lot of experience with real estate properties and working
          with different customers around the world.
        </p>
      </div>
      <div>
        <h3 class="mb-4 text-2xl font-semibold">Information</h3>
        <ul class="flex flex-col space-y-2">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/">Explore</NuxtLink></li>
          <li><NuxtLink to="/">Resources</NuxtLink></li>
          <li><NuxtLink to="/">Contact</NuxtLink></li>
          <li><NuxtLink to="/">Blog</NuxtLink></li>
        </ul>
      </div>
      <div>
        <h3 class="mb-4 text-2xl font-semibold">Helpful links</h3>
        <ul class="flex flex-col space-y-2">
          <li><NuxtLink to="/">Properties</NuxtLink></li>
          <li><NuxtLink to="/">Supports</NuxtLink></li>
          <li><NuxtLink to="/">Terms & Condition</NuxtLink></li>
          <li><NuxtLink to="/">Privacy</NuxtLink></li>
        </ul>
      </div>
      <div>
        <h3 class="mb-4 text-2xl font-semibold">Contact</h3>
        <ul class="flex flex-col space-y-2">
          <li><NuxtLink to="/">+1 8934 21834 23</NuxtLink></li>
          <li><NuxtLink to="/">Restate@gmail.com</NuxtLink></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'TheFooter',
}
</script>

<style scoped>
.footer {
  @apply container mx-auto flex max-w-6xl items-center justify-between;
}
</style>
