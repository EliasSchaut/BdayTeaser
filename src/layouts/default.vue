<template>
  <Body
    class="bg-white text-secondary-900 dark:text-white selection:bg-prime-100 dark:bg-second-900 dark:selection:bg-prime-900"
  />
  <div class="flex flex-col h-screen justify-between">
    <LayoutNav />
    <main class="mb-auto">
      <slot />
    </main>
    <LayoutFooter />
  </div>
</template>
