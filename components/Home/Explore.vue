<script setup>
const cities = [
  {
    name: "🇮🇩 Indonasia",
    size: "big",
  },
  { name: "🇸🇬 Singapore" },
  { name: "🇺🇸 USA", size: "big" },
  { name: "🇫🇷 France" },
];
</script>

<template>
  <section
    class="container mx-auto max-xl:px-8 min-h-screen grid place-items-center grid-cols-2 gap-16"
  >
    <div class="grid justify-items-start content-center gap-8">
      <div class="text-4xl font-bold">
        Let's explore the world with Divy Travel
      </div>
      <div class="space-y-4 text-slate-500">
        <p>
          Traveling can be a great way to explore the world and learn about new
          cultures. What do you want to get out of your trip? Do you want to
          relax on a beach, learn about a new culture, or experience new foods?
          Setting your goals will help you plan your trip and make the most of
          your time.
        </p>
        <p>
          There are so many amazing places to visit, it can be hard to decide
          where to go. Do some research to find a destination that aligns with
          your travel goals and budget.
        </p>
      </div>
      <Button size="lg">Learn more</Button>
    </div>
    <div class="grid grid-cols-2 gap-6">
      <div
        class="relative"
        :class="{ big: size == 'big' }"
        v-for="({ name, size }, index) in cities"
        :key="index"
      >
        <img
          :src="
            'http://picsum.photos/300/' +
            (size == 'big' ? 400 : 250) +
            '.webp?' +
            index
          "
          class="w-full object-cover rounded-2xl"
          alt=""
        />
        <BlurBadge size="sm" class="absolute top-4 left-4">{{
          name
        }}</BlurBadge>
      </div>
    </div>
  </section>
</template>
