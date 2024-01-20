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
    class="flex w-full p-2 bg-white rounded-full overflow-hidden"
  >
    <input
      :type="type ?? 'text'"
      :placeholder="placeholder"
      class="flex-1 px-4 outline-none text-black"
      required
    />
    <Button>{{ label }}</Button>
  </form>
</template>
