<template>
  <section class="my-20">
    <SectionHeading title="Our best blog" />
    <p v-if="$fetchState.pending">Fetching houses...</p>
    <p v-else-if="$fetchState.error">An error occurred :(</p>
    <div v-else class="flex items-center space-x-8">
      <div class="w-1/2">
        <div class="flex flex-col space-y-12">
          <PostCard
            v-for="post in posts"
            :key="post.id"
            :id="post.id"
            :title="post.title"
            :subtitle="post.short_description"
            :date="post.created_at"
            :featuredImage="post.featured_image"
          />
        </div>
      </div>
      <div class="w-1/2">
        <img src="~/assets/images/home01.jpg" alt="" class="rounded-2xl" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BlogPosts',
  data: () => ({
    posts: [],
  }),
  async fetch() {
    this.posts = await this.$axios.$get(`posts/`)
  },
}
</script>

<style scoped></style>
