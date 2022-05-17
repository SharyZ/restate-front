<template>
  <div>
    <h1>profile</h1>
    <button @click="logout">logout</button>
  </div>
</template>

<script>
export default {
  name: 'ProfilePage',
  middleware: ['auth'],
  methods: {
    async logout() {
      await this.$auth.logout()
    },
  },
}
</script>

<style scoped></style>
