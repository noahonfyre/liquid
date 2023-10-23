<template>
  <h1 v-if="large" class="font-bold text-slate-950 text-5xl">
    <slot></slot>
  </h1>

  <h1 v-if="normal" class="font-bold text-slate-950 text-3xl">
    <slot></slot>
  </h1>

  <h1 v-if="small" class="font-bold text-slate-950 text-md">
    <slot></slot>
  </h1>
</template>

<script setup>
defineProps({
  large: {
    type: Boolean,
    default: false
  },
  normal: {
    type: Boolean,
    default: false
  },
  small: {
    type: Boolean,
    default: false
  }
})
</script>