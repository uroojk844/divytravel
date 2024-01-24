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
  <section class="container mx-auto max-lg:px-4 py-12 max-sm:py-4">
    <div class="flex max-sm:flex-wrap items-center justify-between mb-12 max-sm:mb-4 gap-8 max-sm:gap-4">
      <div class="flex gap-4 overflow-x-auto no-scrollbar">
        <div
          v-for="(place, index) in places"
          :key="index"
          class="max-sm:text-sm max-sm:py-2.5 px-6 py-3 rounded-full cursor-pointer hover:bg-blue-500 hover:text-white transition-colors"
          :class="
            filteredPlace == place ? 'bg-blue-500 text-white' : 'bg-blue-100'
          "
          @click="filteredPlace = place"
        >
          {{ place }}
        </div>
      </div>

      <div class="flex gap-2 sm:bg-blue-50 sm:p-1.5 sm:rounded-full">
        <input type="text" placeholder="Search places" class="py-2 px-6 rounded-full outline-none border max-sm:max-w-52 flex-1"/>
        <button class="bg-blue-500 max-sm:text-sm max-sm:w-full max-sm:px-4 px-3 py-2 hover:bg-blue-600 active:scale-95 transition-transform rounded-full text-white">Search</button>
      </div>
    </div>
    <div class="grid max-sm:grid-cols-1 grid-cols-3 gap-6">
      <Card v-for="(item, index) in 'dsjfhsdjk'" :key="index" :data="item" />
    </div>
  </section>
</template>
