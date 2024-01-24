<script setup>
const { type, placeholder, label } = defineProps([
  "type",
  "placeholder",
  "label",
]);
</script>

<template>
  <form
    method="post"
    @submit.prevent=""
    class="flex gap-4 max-sm:flex-wrap w-full max-sm:justify-center sm:p-2 sm:bg-white sm:rounded-full overflow-hidden"
  >
    <input
      :type="type ?? 'text'"
      :placeholder="placeholder"
      class="flex-1 px-3 outline-none text-black max-sm:py-2.5 rounded-full"
      required
    />
    <Button>{{ label }}</Button>
  </form>
</template>
