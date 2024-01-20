<script setup>
const data = [
  {
    icon: "i-tabler:world-search",
    title: "Many destinations",
    desc: "There are many choices of destinations that you can find according to your needs and desires.",
  },
  {
    icon: "i-tabler:credit-card",
    title: "Many payment options",
    desc: "There are many payment methods when you make transactions to order tickets without the hassle.",
  },
  {
    icon: "i-mdi:shield-key-outline",
    title: "Secured transcation",
    desc: "Your payment is safe and protected. We can also process it easily for ticket refunds by waiting a maximum of one day.",
  },
];
</script>

<template>
  <div class="bg-secondary">
    <section
      class="container mx-auto min-h-screen grid content-center justify-items-center max-xl:px-8"
    >
      <div class="text-4xl font-bold mb-4">Why Travely</div>
      <div class="text-slate-500 mb-16">
        There are many advantages to booking your travel tickets over other
        competitors
      </div>

      <div class="grid grid-cols-3 gap-6">
        <div
          class="p-6 bg-white/40 rounded-xl"
          v-for="(item, index) in data"
          :key="index"
        >
          <div
            class="w-[70px] aspect-square grid place-items-center rounded-full bg-secondary mb-4"
          >
            <Icon :name="item.icon" size="36" color="#3575f5" />
          </div>
          <div class="text-2xl font-bold mb-2">{{ item.title }}</div>
          <div class="text-sm text-slate-500">{{ item.desc }}</div>
        </div>
      </div>
    </section>
  </div>
</template>
