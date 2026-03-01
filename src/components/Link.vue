<script setup>
const props = defineProps({
  active: Boolean,
})
</script>

<template>
  <a
    class="flex items-center px-3.5 h-10 text-white text-sm font-medium rounded-full transition duration-300 cursor-pointer"
    :class="active ? 'bg-white/30 backdrop-blur-md border border-white/40' : ''"
  >
    <slot />
  </a>
</template>
