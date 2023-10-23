<template>
  <NuxtLink class="text-indigo-600 font-bold" :to="target">
    <slot></slot>
  </NuxtLink>
</template>

<script setup>
defineProps({
  target: {
    type: String,
    default: "/"
  }
})
</script>