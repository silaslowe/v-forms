<template>
  <label>{{ label }}</label>
  <input v-bind="$attrs" :placeholder="label" class="field" :value="modelValue" @input="$emit('update:modelValue', $event.target.vaule)"  />
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      defaule: ''
    },
    modelValue: {
      type: [String, Number],
      default: ''
    }
  }
}
</script>
