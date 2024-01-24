<template>
  <section class="grid grid-cols-2 max-sm:grid-cols-1">
    <div
      class="max-sm:min-h-svh bg-primary grid place-content-center place-items-center gap-8 px-12 py-16"
    >
      <div class="flex items-center gap-5 flex-col text-4xl font-bold">
        <div class="flex relative w-24">
          <div class="w-12 aspect-square bg-blue-700 rounded-full"></div>
          <div
            class="absolute right-3 w-12 aspect-square bg-orange-200 rounded-full"
          ></div>
        </div>
        DivyTravel
      </div>
      <div class="text-6xl max-sm:text-3xl max-w-md text-center font-semibold">
        We love to hear your valuable feedback.
      </div>
    </div>


    <div class="bg-blue-100 grid place-items-center py-24 px-4">
      <form
        method="post"
        class="bg-white px-8 max-sm:px-4 py-12 rounded-3xl shadow-md grid gap-6 max-w-md w-full mx-auto"
        @submit.prevent=""
      >
        <div class="group">
          <input type="text" placeholder=" " required />
          <label>Full name</label>
        </div>
        <div class="group">
          <input type="email" placeholder=" " required />
          <label>Email address</label>
        </div>
        <div class="group">
          <input
            type="tel"
            placeholder=" "
            minlength="10"
            maxlength="10"
            required
          />
          <label>Mobile number</label>
        </div>
        <div class="group">
          <textarea rows="5" placeholder=" " required></textarea>
          <label>Your message</label>
        </div>
        <Button>Submit</Button>
      </form>
    </div>
  </section>
</template>

<style scoped>
.group {
  display: grid;
  gap: 4px;
  position: relative;
}

label {
  position: absolute;
  color: rgba(112, 128, 144, 0.813);
  transform: translate(17px, 13px);
  pointer-events: none;
  transition: 300ms ease;
}

form :is(input, textarea) {
  border: 1px solid #e5e5e5;
  outline: transparent;
  border-radius: 12px;
  padding: 12px 16px;
  caret-color: dodgerblue;
}

form :is(input, textarea):focus + label,
form :is(input, textarea):not(:placeholder-shown) + label {
  transform: translate(16px, -50%);
  font-size: 10px;
  background-color: var(--primary);
  color: white;
  padding: 2px 8px;
  border-radius: 8px;
  letter-spacing: 1px;
}
</style>
