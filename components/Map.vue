<template>
    <section class="map">
        <div class="map__container _container">
            <div class="map__body min-h-[1123px]">

                <div class="outer__ticket max-w-[825px] mb-[185px]">
                    <GreyTicketMap class="mb-[185px]">
                    </GreyTicketMap>
                </div>

                <div class="flex flex-wrap gap-y-[60px] gap-x-[74px] xl:gap-y-[170px] justify-center">
                    <MapCard Subtitle="Направление 1" Paragraph="Рассказываем бизнесу о методах привлечения финансирования"></MapCard>
                    <MapCard Subtitle="Направление 2" Paragraph="ТОСЭР. Поддержка приоритетных направлений, антикризисные меры. Инфраструктурные проекты."></MapCard>
                    <MapCard Subtitle="Направление 3" Paragraph="Гранты для начинающих фермеров. Субсидии действующим предпринимателям. Субсидирование кредитов."></MapCard>
                    <MapCard Subtitle="Направление 4" Paragraph="Возмещение затрат по приоритетным направлениям. Возмещение затрат на пилотные партии. Поддержка инноваций."></MapCard>
                    <MapCard Subtitle="Направление 5" Paragraph="Гарантийная поддержка. Льготное кредитования. Льготный лизинг. Информационная поддержка."></MapCard>
                    <MapCard Subtitle="Направление 6" Paragraph="Возвратные средства 0-5%. Инфраструктурные проекты."></MapCard>
                    <MapCard Subtitle="Направление 7" Paragraph="Возмещение транспортных затрат. Возмещение затрат на выставки. Субсидирование кредитов по экспортным контрактам."></MapCard>
                    <MapCard Subtitle="Направление 8" Paragraph="Возмещение затрат по приоритетным направлениям. Возмещение затрат на пилотные партии. Поддержка инноваций."></MapCard>
                </div>
                

            </div>
        </div>
    </section>
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
<style lang="scss">
.map {
    background: no-repeat center url("~/assets/img/map/backgoundTest.jpg");
}

</style>