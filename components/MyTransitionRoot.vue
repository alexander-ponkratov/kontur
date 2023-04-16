<template>
  <TransitionRoot appear :show=true enter="transition-opacity duration-1000" enter-from="opacity-0" enter-to="opacity-100"
    leave="transition-opacity duration-1000" leave-from="opacity-100" leave-to="opacity-0">
    <slot></slot>
  </TransitionRoot>
</template>


<!-- component script -->
<script lang="ts">
export default {
  /* passed props */
  props: {
    ImageSrc: String,
    ImageAlt: String,
  },
  /*     data: () => ({
      }), */
  /* js code */
  mounted() {
  },
  methods: {
  }
}
</script>

<!-- About Nuxt 3 bug: https://github.com/nuxt/nuxt/issues/14766 -->
<script setup lang="ts">

/* import for transition to work */
import { TransitionRoot } from '@headlessui/vue'

/* use images as props:
<img :src="useAsset(ImageSrc + '')"  :alt="ImageAlt" class="collection__image"> 
*/
function useAsset(path: string): string {
  const assets = import.meta.glob('~/assets/**/*', {
    eager: true,
    import: 'default',
  })
  // @ts-expect-error: wrong type info
  return assets['/assets/' + path]
}


</script>

<!-- component style -->
<style lang="scss"></style>