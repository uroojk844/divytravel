<script setup>
const { size } = defineProps({
  size: {
    default: "md",
  },
});
</script>

<template>
  <button
    class="button outline-transparent bg-primary text-nowrap hover:bg-blue-600 active:scale-95 transition-transform rounded-full text-sm"
    :class="[{ 'px-6 py-3': size == 'md' }, { 'py-4 px-8': size == 'lg' }]"
  >
    <slot></slot>
  </button>
</template>
