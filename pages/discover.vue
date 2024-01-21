<script setup>
const filteredPlace = ref("All");
const places = [
  "All",
  "USA",
  "Indonesia",
  "France",
  "Germany",
  "India",
  "Italy",
];
</script>

<template>
  <section class="container mx-auto max-lg:px-8 py-12">
    <div class="flex items-center justify-between mb-12 gap-8">
      <div class="flex gap-4 overflow-x-auto no-scrollbar">
        <div
          v-for="(place, index) in places"
          :key="index"
          class="px-6 py-3 rounded-full cursor-pointer hover:bg-blue-500 hover:text-white transition-colors"
          :class="
            filteredPlace == place ? 'bg-blue-500 text-white' : 'bg-blue-100'
          "
          @click="filteredPlace = place"
        >
          {{ place }}
        </div>
      </div>

      <div class="flex gap-2 bg-blue-50 p-1.5 rounded-full">
        <input type="text" placeholder="Search places" class="py-2 px-6 rounded-full outline-none"/>
        <button class="bg-blue-500 px-3 py-2 hover:bg-blue-600 active:scale-95 transition-transform rounded-full text-white">Search</button>
      </div>
    </div>
    <div class="grid grid-cols-3 gap-6">
      <Card v-for="(item, index) in 'dsjfhsdjk'" :key="index" :data="item" />
    </div>
  </section>
</template>
