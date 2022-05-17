<template>
  <div class="form-control">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'FormControl',

  data() {
    return {}
  },
}
</script>

<style lang="css" scoped>
.form-control {
  @apply mb-4;
}
</style>
