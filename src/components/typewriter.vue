<template>
  <span id="typewriter" ref="target" class="font-bold text-pink-500 dark:text-pink-400" />
</template>

<script lang="ts">
import Typewriter from 'typewriter-effect/dist/core';
import { useElementVisibility } from '@vueuse/core'

export default defineComponent({
  setup() {
    const typewriter = ref<HTMLElement | null>(null)
    return {
      typewriter,
      target_is_visible: useElementVisibility(typewriter) as Ref<boolean>,
    }
  },
  mounted() {
    new Typewriter('#typewriter', {
      strings: this.strings,
      loop: true,
      autoStart: true,
    });
    this.typewriter = this.$refs.target as HTMLElement;
    watch(this.target_is_visible, this.on_element_visibility)
  },
  methods: {
    on_element_visibility(is_visible: boolean) {
      if (is_visible) {
        this.play()
        console.log("play")
      } else {
        this.pause()
        console.log("pause")
      }
    },
    pause() {
      this.typewriter!.stop()
    },
    play() {
      this.typewriter!.start()
    },
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
