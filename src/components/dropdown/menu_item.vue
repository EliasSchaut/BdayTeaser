<template>
  <MenuItem
    as="div"
    class="text-sm text-second-700 hover:bg-second-100 dark:text-second-400 dark:hover:bg-second-900"
  >
    <slot />
  </MenuItem>
</template>

<script setup lang="ts">
import { MenuItem } from '@headlessui/vue';
</script>
