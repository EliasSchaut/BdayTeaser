<template>
  <!-- hero -->
  <div class="pb-16 pt-20 text-center dark:text-white lg:pt-32">
    <h1
      class="font-display mx-auto max-w-4xl text-5xl font-medium tracking-tight text-slate-900 sm:text-7xl"
    >
      <span>Save </span>
      <Underline>the DATE</Underline>
    </h1>
    <p class="mx-auto mt-6 max-w-2xl text-lg tracking-tight text-slate-700">
      Am
      <Accent>07. Juni 2025</Accent>
      steigt die Geburtstagsparty des Jahres! Also haltet euch den Termin frei
      und seid dabei!
    </p>
  </div>

  <!-- newsletter -->
  <div id="newsletter" class="py-16 sm:py-24">
    <div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
      <div
        class="relative isolate overflow-hidden bg-second-950 px-6 py-24 shadow-2xl sm:rounded-3xl sm:px-24 xl:py-32"
      >
        <h2
          class="mx-auto max-w-3xl text-center text-4xl font-semibold tracking-tight text-white sm:text-5xl"
        >
          Get notified when the registration is open
        </h2>
        <p class="mx-auto mt-6 max-w-lg text-center text-lg text-second-300">
          Du möchtest nichts verpassen? Sign up for the bday newsletter! We
          care about your data. Read our
          <a class="font-bold hover:underline" href="/privacy">privacy policy</a
          >.
        </p>
        <form
          class="mx-auto mt-10 flex max-w-md gap-x-4"
          action="https://axolotlens.us8.list-manage.com/subscribe/post?u=f82527e01ab3b8bc7d058d779&amp;id=5d17f9332f&amp;f_id=006967e1f0"
          method="post"
        >
          <label for="email-address" class="sr-only">Email address</label>
          <input
            class="min-w-0 flex-auto rounded-md bg-white/5 px-3.5 py-2 text-base text-white outline-1 -outline-offset-1 outline-white/10 placeholder:text-second-400 focus:outline-2 focus:-outline-offset-2 focus:outline-white sm:text-sm/6"
            id="mce-EMAIL"
            type="email"
            name="EMAIL"
            autocomplete="email"
            placeholder="Enter your email"
            required
          />
          <button
            type="submit"
            class="shadow-xs flex-none rounded-md bg-white px-3.5 py-2.5 text-sm font-semibold text-second-900 hover:bg-second-100 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-white"
          >
            Notify me
          </button>
        </form>
        <svg
          viewBox="0 0 1024 1024"
          class="absolute left-1/2 top-1/2 -z-10 size-[64rem] -translate-x-1/2"
          aria-hidden="true"
        >
          <circle
            cx="512"
            cy="512"
            r="512"
            fill="url(#759c1415-0410-454c-8f7c-9a820de03641)"
            fill-opacity="0.7"
          />
          <defs>
            <radialGradient
              id="759c1415-0410-454c-8f7c-9a820de03641"
              cx="0"
              cy="0"
              r="1"
              gradientUnits="userSpaceOnUse"
              gradientTransform="translate(512 512) rotate(90) scale(512)"
            >
              <stop stop-color="#7775D6" />
              <stop offset="1" stop-color="#E935C1" stop-opacity="0" />
            </radialGradient>
          </defs>
        </svg>
      </div>
    </div>
  </div>
</template>
