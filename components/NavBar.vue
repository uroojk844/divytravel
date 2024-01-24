<script setup></script>

<template>
  <div class="border-b">
    <nav
      class="container mx-auto max-xl:px-8 py-4 flex justify-between items-stretch"
      :class="{
        'text-gray-50 absolute z-10 top-0 left-1/2 -translate-x-1/2': [
          '/',
        ].includes($route.path),
      }"
    >
      <Logo />
      <div class="flex gap-2 capitalize relative max-sm:hidden">
        <NuxtLink class="p-6" to="/">home</NuxtLink>
        <NuxtLink class="p-6" to="/discover">discover</NuxtLink>
        <NuxtLink class="p-6" to="/about">about</NuxtLink>
        <NuxtLink class="p-6" to="/contact">contact</NuxtLink>
      </div>
    </nav>
  </div>
</template>