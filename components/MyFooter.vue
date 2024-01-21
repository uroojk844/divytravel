<template>
  <div class="border-t">
    <section class="container mx-auto max-xl:px-8">
      <footer class="flex justify-between py-8">
        <div class="grid gap-4">
          <Logo />
          <p class="text-slate-500 mb-6 max-w-64">
            Search deals on hotels, homes, and much more.
          </p>
          <div class="flex items-center gap-2 text-slate-500">
            <Icon name="ri:instagram-fill" size="22" />
            <Icon name="ion:social-facebook" size="22" />
            <Icon name="basil:linkedin-solid" size="22" />
            <Icon name="ri:twitter-x-fill" size="22" />
          </div>
        </div>
        <div class="">
          <div class="text-lg font-bold mb-2">Quick links</div>
          <div class="grid gap-2 text-sm">
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/discover">Discover</NuxtLink>
            <NuxtLink to="/about">About</NuxtLink>
            <NuxtLink to="/contact">Contact</NuxtLink>
          </div>
        </div>
        <div class="">
          <div class="text-lg font-bold mb-2">Support</div>
          <div class="grid gap-2 text-sm">
            <NuxtLink to="/help">Help Center</NuxtLink>
            <NuxtLink to="/contact">Contact us</NuxtLink>
          </div>
        </div>
        <div class="">
          <div class="text-lg font-bold mb-2">Contact us</div>
          <div class="grid gap-2 text-sm">
            <div class="max-w-64">
              Dvya Travel, Varanasi, Uttar Pradesh, 221210
            </div>
            <div>+918114076364</div>
            <div>uroojk844@gmail.com</div>
          </div>
        </div>
      </footer>
      <div class="flex items-center justify-between py-8 text-sm">
        <div>&copy; Copyright {{ new Date().getFullYear() }} Divy Travel</div>
        <div class="flex gap-6">
          <div>Terms & Condition</div>
          <div>Privacy &Policy</div>
        </div>
      </div>
    </section>
  </div>
</template>
