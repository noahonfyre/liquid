<template>
  <div class="bg-slate-50 text-slate-400 ring-1 ring-inset ring-slate-200 rounded-lg flex gap-3 items-center justify-stretch py-2 px-4 shadow-md ease-in-out duration-300 focus-within:ring-2 focus-within:ring-indigo-600 focus-within:text-indigo-600">
    <slot></slot>
    <input :type="type" :placeholder="placeholder" class="w-full text-center placeholder-slate-400 focus:placeholder-transparent placeholder:font-normal font-medium text-sm text-slate-600 bg-transparent focus-visible:outline-none">
  </div>
</template>
<script setup>
defineProps({
  type: {
    type: String,
    default: "text"
  },
  placeholder: {
    type: String,
    default: "Enter something."
  }
})
</script>