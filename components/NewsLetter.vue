<template>
  <section class="container mx-auto max-sm:px-4 max-xl:px-8 py-16">
    <div class="flex flex-wrap justify-between items-center max-sm:px-6 max-sm:py-12 p-16 bg-primary rounded-xl">
      <div class="space-y-5 max-sm:mb-4">
        <div class="text-3xl font-bold">Get our best offer now</div>
        <div>Sign up and we'll send the best deals to you</div>
      </div>
      <SingleFieldForm
        type="email"
        class="max-w-md"
        placeholder="Your email address"
        label="Subscribe now"
      />
    </div>
  </section>
</template>
