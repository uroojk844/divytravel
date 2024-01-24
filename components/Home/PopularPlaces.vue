<script setup>
defineProps({
  items: {
    default: [1, 2, 3],
  },
});
</script>

<template>
  <section class="container mx-auto max-xl:px-8 py-16">
    <div class="flex justify-between items-end mb-8">
      <div class="space-y-3">
        <div class="text-3xl font-bold">Popular destination</div>
        <div class="text-sm text-slate-500">Recommendation place for you</div>
      </div>
      <NuxtLink class="max-sm:hidden" to="/discover">
        <Button>See all destination</Button>
      </NuxtLink>
    </div>

    <div class="grid grid-cols-3 max-sm:grid-cols-1 gap-6 max-sm:mb-8">
      <Card v-for="(item, index) in $props.items" :key="index" :data="item" />
    </div>

    <NuxtLink class="sm:hidden flex justify-center" to="/discover">
      <Button>See all destination</Button>
    </NuxtLink>
  </section>
</template>
