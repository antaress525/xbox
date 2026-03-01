<script setup>
defineProps({
  variant: {
    type: String,
    default: 'primary', // primary secondary
  },
})
</script>

<template>
  <button
    class="flex items-center cursor-pointer gap-2 px-3.5 h-9 text-sm rounded-full"
    :class="variant === 'primary' ? 'bg-white text-black' : 'bg-black/25 text-white'"
  >
    <slot />
  </button>
</template>
