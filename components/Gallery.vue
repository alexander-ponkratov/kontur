<template>
    <section class="relative gallery min-h-[890px]">
        <div class="gallery__container _container">
            <div class=" gallery__body ">
                <H1 class="!text-[42px] text-center mb-[80px]">Галерея</H1>
                <div
                    class="gallery__items flex flex-wrap gap-y-[45px] gap-x-[57px] max-w-[1226px] justify-center my-0 mx-auto">
                    <GalleryImg ImageSrc="img/gallery/01.jpg" ImageAlt="01"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/02.jpg" ImageAlt="02"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/03.jpg" ImageAlt="03"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/04.jpg" ImageAlt="04"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/05.jpg" ImageAlt="05"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/06.jpg" ImageAlt="06"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/07.jpg" ImageAlt="07"></GalleryImg>
                    <GalleryImg ImageSrc="img/gallery/08.jpg" ImageAlt="08"></GalleryImg>
                </div>
                <div class="gallery__dotsW"><img src="~/assets/img/gallery/dots.png" alt="dots"
                        class="gallery__dots absolute bottom-5 right-5"></div>
            </div>
        </div>
    </section>
</template>


<!-- component script -->
<script>
export default {
    /* passed props */
    props: {
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

<!-- component style -->
<style lang="scss"></style>