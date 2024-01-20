<template>
  <nav
    class="text-gray-50 absolute top-0 left-1/2 -translate-x-1/2 container py-6 flex justify-between items-center"
  >
    <div class="flex items-center gap-3 text-xl font-medium">
      <div class="flex relative w-11">
        <div class="w-6 aspect-square bg-blue-700 rounded-full"></div>
        <div class="absolute right-0 w-6 aspect-square bg-orange-200 rounded-full"></div>
      </div>
      DivyTravel
    </div>
    <div class="flex gap-8 font-medium capitalize">
      <NuxtLink to="/">home</NuxtLink>
      <NuxtLink to="/about">about</NuxtLink>
      <NuxtLink to="/contact">contact</NuxtLink>
    </div>
  </nav>
</template>
