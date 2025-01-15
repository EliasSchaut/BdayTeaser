<template>
  <span id="typewriter" class="font-bold text-pink-500 dark:text-pink-400" />
</template>

<script lang="ts">
import Typewriter from 'typewriter-effect/dist/core';

export default defineComponent({
  mounted() {
    new Typewriter('#typewriter', {
      strings: this.strings,
      loop: true,
      autoStart: true,
    });
  },
  props: {
    heading: {
      type: String,
      default: '',
    },
    strings: {
      type: Array<String>,
      required: true,
    },
  },
});
</script>
