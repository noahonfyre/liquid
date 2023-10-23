<template>
  <div class="flex flex-col gap-3">
    <LiquidHeading normal>{{ heading }}</LiquidHeading>
    <div class="flex items-center gap-3 bg-slate-50 rounded-3xl p-8">
      <slot></slot>
    </div>
  </div>
</template>

<script setup>
defineProps({
  heading: {
    type: String,
    default: "No heading provided."
  }
})
</script>