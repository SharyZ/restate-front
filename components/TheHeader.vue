<template>
  <header class="header">
    <NuxtLink to="/">
      <TheLogo />
    </NuxtLink>
    <TheNavbar />
    <div v-if="loggedIn" class="flex items-center space-x-4">
      <NuxtLink to="/profile" class="py-2 px-4 text-lg font-semibold">
        Hi, @{{ username }}
      </NuxtLink>
      <NuxtLink
        to=""
        @click.native="logout"
        class="py-2 px-4 text-lg font-semibold"
        title="Logout"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1"
          />
        </svg>
      </NuxtLink>
    </div>
    <div v-else class="flex items-center space-x-4">
      <NuxtLink to="/login" class="py-2 px-4 text-lg font-semibold">
        Login
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
  methods: {
    async logout() {
      await this.$auth.logout()
    },
  },
  computed: {
    loggedIn() {
      return this.$auth.user
    },
    username() {
      return this.$auth.user.username
    },
  },
}
</script>

<style scoped>
.header {
  @apply flex items-center justify-between py-6 px-4;
}
</style>
