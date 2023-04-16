<template>
    <div class="galleryImgW"><img :src="useAsset(ImageSrc + '')"  :alt="ImageAlt" class="galleryImg z-10 relative"></div>
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
<!--usage <img :src="useAsset(ImageSrc + '')"  :alt="ImageAlt" class="collection__image"> -->
<script setup lang="ts">
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