<script setup>
const { data } = defineProps(["data"]);
</script>

<template>
  <div class="rounded-2xl overflow-hidden shadow-sm">
    <img
      :src="'http://picsum.photos/400.webp?' + data"
      class="w-full object-cover max-sm:aspect-video"
      alt=""
    />
    <div class="p-5">
      <div class="text-xl font-semibold">Beach walk badung</div>
      <div class="text-sm mb-4">Bali, Indonesia</div>
      <div class="flex gap-2 items-center mb-2">
        <div class="text-xs px-2 py-1 bg-zinc-100 rounded-sm text-red-700">
          12%
        </div>
        <div class="line-through text-sm text-slate-500">$694</div>
      </div>
      <div>
        <span class="font-bold text-xl">$498</span>
        <span class="text-slate-500">/night</span>
      </div>
    </div>
  </div>
</template>
