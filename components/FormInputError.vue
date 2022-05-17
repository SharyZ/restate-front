<template>
  <div class="form-input-error">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'FormInputError',

  data() {
    return {}
  },
}
</script>

<style lang="css" scoped>
.form-input-error {
  @apply text-sm font-medium text-red-500;
}
</style>
