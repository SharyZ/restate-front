<template>
  <button class="form-button" type="submit">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: 'FormButton',

  data() {
    return {}
  },
}
</script>

<style lang="css" scoped>
.form-button {
  @apply mx-auto mb-2 mt-2 block w-auto rounded-lg bg-rose-500 p-3 py-2 px-4 text-lg font-semibold text-white;
}
</style>
