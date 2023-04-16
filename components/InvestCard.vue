<template>
    <div class="pt-[69px] pr-[55px] pb-[72px] pl-[30px] bg-white flex flex-col invest__card m-3 mt-[-5px]">
        <div class="card__imgW"><img :src="useAsset(ImageSrc + '')" :alt="ImageAlt" class="card__img mb-[49px]"></div>
        <P class="font-semibold mb-[20px]">{{ Subtitle }}</P>
        <P class="font-normal max-w-[269px]">{{ Paragraph }}</P>
    </div>
</template>


<!-- component script -->
<script lang="ts">
export default {
    /* passed props */
    props: {
        ImageSrc: String,
        ImageAlt: String,
        Subtitle: String,
        Paragraph: String,
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
<style lang="scss">
.invest__card {
    background: #FFFFFF;
    border: 1px solid #EEEEEE;
    box-shadow: 0px 6px 44px -12px rgba(97, 97, 97, 0.1), 0px 16px 32px 2px rgba(97, 97, 97, 0.15);
    border-radius: 16px;
}
</style>