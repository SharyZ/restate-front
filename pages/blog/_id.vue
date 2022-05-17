<template>
  <div class="mx-auto mb-10 max-w-3xl">
    <div class="mb-10">
      <h2 class="mb-4 text-4xl font-black">{{ post.title }}</h2>
      <p class="flex items-center space-x-2 font-semibold text-rose-500">
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
            d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
          />
        </svg>
        <span>{{ post.created_at | formatDate }}</span>
      </p>
    </div>
    <img :src="post.featured_image" alt="" class="mb-10 rounded-2xl" />
    <div v-html="post.full_description"></div>
  </div>
</template>

<script>
export default {
  name: 'BlogPost',
  async asyncData({ params, $axios }) {
    const post = await $axios.$get(`posts/${params.id}`)
    return { post }
  },
}
</script>

<style scoped></style>
