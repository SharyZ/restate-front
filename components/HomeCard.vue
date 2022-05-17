<template>
  <div class="overflow-hidden rounded-2xl">
    <img :src="featuredImage" alt="" />
    <div class="mb-4 p-4">
      <div class="flex items-center space-x-4">
        <div class="flex-grow">
          <h3 class="mb-2 text-4xl font-semibold">${{ price }}</h3>
          <p>{{ address }}, {{ city }}</p>
        </div>
        <div
          class="rounded-md bg-blue-200 px-2 py-1 font-semibold text-blue-900"
        >
          {{ saleType }}
        </div>
      </div>
    </div>
    <NuxtLink
      :to="'/explore/' + id"
      class="block w-full bg-rose-400 p-2 text-center font-semibold text-white"
    >
      View details
    </NuxtLink>
  </div>
</template>

<script>
export default {
  name: 'HomeCard',
  props: {
    id: {
      type: Number,
    },
    price: {
      type: Number,
    },
    address: {
      type: String,
    },
    city: {
      type: String,
    },
    saleType: {
      type: String,
    },
    featuredImage: {
      type: String,
      required: true,
      default: '',
    },
  },
}
</script>
