<template>
    <div class="face__carousel flex max-w-[1128px]">
        <div class="face__carouselImgW"><img src="~/assets/img/face/01.png" alt="01" class="face__carousel"></div>
        <div class="face__carouselImgW"><img src="~/assets/img/face/02.png" alt="01" class="face__carousel"></div>
        <div class="face__carouselImgW"><img src="~/assets/img/face/03.png" alt="01" class="face__carousel"></div>
        <div class="face__carouselImgW"><img src="~/assets/img/face/04.png" alt="01" class="face__carousel"></div>
        <div class="face__carouselImgW"><img src="~/assets/img/face/05.png" alt="01" class="face__carousel"></div>

    </div>
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
        $(document).ready(function () {
            $(".face__carousel").slick({
                infinite: true,
                slidesToShow: 4,
                slidesToScroll: 4,
                prevArrow: "<img src=\"/_nuxt/assets/img/face/prev.svg\" alt=\"prev\" class=\"prev\">",
                nextArrow: "<img src=\"/_nuxt/assets/img/face/next.svg\" alt=\"next\" class=\"next\">",
                responsive: [
                    {
                        breakpoint: 767,
                        settings: {
                            slidesToShow: 2,
                            slidesToScroll: 2
                        }
                    },
                    {
                        breakpoint: 576,
                        settings: {
                            slidesToShow: 1,
                            slidesToScroll: 1
                        }
                    }
                ]
            });
        });
    },
    methods: {
    }
}
</script>

<!-- component style -->
<style lang="scss">
.face__carouselImgW{
    height: 91px;
    display: flex !important;
    justify-content: center;
    align-items: center;
}
</style>