<script setup>
defineProps({
  size: {
    default: "md",
  },
});
</script>

<template>
  <div
    class="text-sm bg-black/10 backdrop-blur-3xl text-white rounded-full"
    :class="[{ 'py-2.5 px-6': size == 'md' }, { 'py-1 px-3': size == 'sm' }]"
  >
    <slot></slot>
  </div>
</template>
