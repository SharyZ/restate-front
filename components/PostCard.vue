<template>
  <NuxtLink to="/" class="flex space-x-4">
    <img
      src="~/assets/images/home02.jpg"
      alt=""
      class="h-40 w-40 rounded-2xl"
    />
    <div>
      <h4 class="mb-4 text-2xl font-semibold">
        {{ title }}
      </h4>
      <p class="mb-2">
        {{ subtitle }}
      </p>
      <p class="text-rose-500">{{ date }}</p>
    </div>
  </NuxtLink>
</template>

<script>
export default {
  name: 'PostCard',
  props: {
    title: {
      type: String,
      required: true,
      default: '',
    },
    subtitle: {
      type: String,
      required: true,
      default: '',
    },
    date: {
      type: String,
      required: true,
      default: '',
    },
  },
}
</script>

<style lang="scss" scoped></style>
