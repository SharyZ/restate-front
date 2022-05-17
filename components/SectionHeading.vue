<template>
  <div class="section-heading">
    <h2 class="title">{{ title }}</h2>
    <p v-if="subtitle" class="subtitle">{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  name: 'SectionHeading',
  props: {
    title: {
      type: String,
      required: true,
      default: '',
    },
    subtitle: {
      type: String,
      required: false,
      default: '',
    },
  },
}
</script>

<style scoped>
.section-heading {
  @apply mb-8 text-center;
}

.title {
  @apply mb-4 text-5xl font-semibold leading-[60px];
}

.subtitle {
  @apply mb-8 text-lg font-medium;
}
</style>
