<template>
  <div class="text-center">
    <slot name="icon"></slot>
    <div class="mb-4 p-4">
      <h3 class="mb-2 text-3xl font-semibold">{{ title }}</h3>
      <p>
        {{ subtitle }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ServiceCard',
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
  },
}
</script>

<style scoped></style>
