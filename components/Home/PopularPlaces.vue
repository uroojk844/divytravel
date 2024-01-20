<template>
  <section class="container mx-auto max-xl:px-8 py-16">
    <div class="flex justify-between items-end mb-8">
      <div class="space-y-3">
        <div class="text-3xl font-bold">Popular destination</div>
        <div class="text-sm text-slate-500">Recommendation place for you</div>
      </div>

      <Button>See all destination</Button>
    </div>

    <div class="grid grid-cols-3 gap-6">
      <Card v-for="(item, index) in [1, 2, 3]" :key="index" :data="item" />
    </div>
  </section>
</template>
