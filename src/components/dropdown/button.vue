<template>
  <MenuButton
    class="shadow-xs rounded-md bg-prime-600 px-3.5 py-2.5 text-sm font-semibold text-white hover:bg-prime-500 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-prime-600"
  >
    <slot />
  </MenuButton>
</template>

<script setup lang="ts">
import { MenuButton } from '@headlessui/vue';
</script>
