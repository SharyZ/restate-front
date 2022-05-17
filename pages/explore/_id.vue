<template>
  <div class="mx-auto mb-10 max-w-3xl">
    <div class="mb-4 flex items-center justify-between">
      <div>
        <h2 class="mb-4 text-4xl font-black">${{ house.price }}</h2>
        <p>{{ house.address }}, {{ house.city }}</p>
      </div>
      <div
        class="inline-block rounded-md bg-blue-200 px-2 py-1 font-semibold text-blue-900"
      >
        {{ house.sale_type }}
      </div>
    </div>
    <img :src="house.featured_image" alt="" class="mb-10 rounded-2xl" />
    <div v-html="house.description"></div>
  </div>
</template>

<script>
export default {
  name: 'SingleHouse',
  async asyncData({ params, $axios }) {
    const house = await $axios.$get(`listings/${params.id}`)
    return { house }
  },
}
</script>

<style scoped></style>
