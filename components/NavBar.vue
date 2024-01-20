<template>
  <nav
    class="text-gray-50 absolute z-10 top-0 left-1/2 -translate-x-1/2 container max-xl:px-8 py-6 flex justify-between items-center"
  >
    <Logo />
    <div class="flex gap-8 capitalize">
      <NuxtLink to="/">home</NuxtLink>
      <NuxtLink to="/discover">discover</NuxtLink>
      <NuxtLink to="/about">about</NuxtLink>
      <NuxtLink to="/contact">contact</NuxtLink>
    </div>
  </nav>
</template>
