<template>
  <label class="form-label">
    <slot></slot>
  </label>
</template>

<script>
export default {
  name: 'FormLabel',

  data() {
    return {}
  },
}
</script>

<style lang="css" scoped>
.form-label {
  @apply mb-2 block text-lg font-medium;
}
</style>
