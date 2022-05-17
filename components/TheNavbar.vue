<template>
  <nav>
    <ul class="nav-list">
      <li
        v-for="navItem in navItems"
        :key="navItem.label"
        class="nav-list-item"
      >
        <NuxtLink :to="navItem.path">{{ navItem.label }}</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'TheNavbar',
  data() {
    return {
      navItems: [
        { path: '/', label: 'Home' },
        { path: '/explore', label: 'Explore' },
        { path: '/resources', label: 'Resources' },
        { path: '/contact', label: 'Contact' },
        { path: '/blog', label: 'Blog' },
      ],
    }
  },
}
</script>

<style scoped>
.nav-list {
  @apply flex items-center space-x-12;
}

.nav-list-item {
  @apply py-1 px-2 text-lg font-semibold;
}

.nav-list-item .nuxt-link-active {
  @apply border-b-2 border-blue-900;
}
</style>
