<template>
  <input
    class="form-input"
    :value="value"
    @input="updateValue($event.target.value)"
  />
</template>

<script>
export default {
  name: 'FormInput',

  props: {
    value: {
      type: String,
    },
  },

  methods: {
    updateValue(value) {
      this.$emit('input', value)
    },
  },
}
</script>

<style lang="css" scoped>
.form-input {
  @apply mb-2 w-full rounded border-none bg-white p-3 shadow-md placeholder:text-slate-400 focus:ring-2 focus:ring-blue-500;
}
</style>
