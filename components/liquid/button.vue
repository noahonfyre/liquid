<template>
  <button @click="action()" v-if="primary" :class="{ 'bg-red-500': color === 'red', 'bg-yellow-400 text-neutral-950': color === 'yellow', 'bg-indigo-600': color === 'default'}" class="text-sm hover:cursor-pointer text-indigo-50 font-medium flex items-center gap-2 px-4 py-2 rounded-lg ease-in-out duration-150 shadow-md">
    <slot></slot>
  </button>

  <button @click="action()" v-if="secondary" class="text-sm hover:cursor-pointer ring-1 ring-inset ring-slate-300 text-neutral-950 font-medium flex items-center gap-2 bg-slate-100 px-4 py-2 rounded-lg ease-in-out duration-150 hover:bg-slate-200 shadow-md">
    <slot></slot>
  </button>

  <button @click="action()" v-if="tertiary" class="text-sm hover:cursor-pointer text-neutral-950 font-semibold flex items-center gap-2 px-4 py-2 rounded-lg ease-in-out duration-150 hover:text-neutral-800">
    <slot></slot>
  </button>
</template>

<script setup>
defineProps({
  action: {
    type: Function,
    default: null
  },
  color: {
    type: String,
    default: "default"
  },
  primary: {
    type: Boolean,
    default: false
  },
  secondary: {
    type: Boolean,
    default: false
  },
  tertiary: {
    type: Boolean,
    default: false
  }
})
</script>