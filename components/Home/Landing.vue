<template>
  <section
    class="min-h-screen text-white relative grid content-center justify-center justify-items-center gap-5 max-sm:p-4"
  >
    <img
      src="~/assets/images/bg.webp"
      class="-z-10 absolute h-full object-cover w-full"
      alt=""
    />
    <BlurBadge>Best travel platform in 2023 ⚡🤩</BlurBadge>
    <div class="text-[56px] font-bold max-sm:text-3xl text-center">Where will your travel take you?</div>
    <div class="sm:text-xl max-sm:text-center">Search deals on hotels, homes, and much more...</div>
    <SingleFieldForm
      type="search"
      class="max-w-lg mt-6"
      placeholder="Search your trip..."
      label="Search places"
    />
  </section>
</template>
