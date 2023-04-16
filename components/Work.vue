<template>
    <section class="relative work">
        <div class="work__container _container">
            <div class="work__body lg:flex gap-x-24 mb-3 lg:mb-0">
                <div class="work__macW"><img src="~/assets/img/work/mac.png" alt="mac" class="work__mac mt-3 lg:mt-[-7.8vw]"></div>

                <div class="text-white">

                    <WhiteTicket class=""></WhiteTicket>

                    <P class="mb-10 max-w-[372px] text-white">Brigth Plan помогает выстроить эффективное взаимодействие с клиентами на всех этапах работы и осуществляет индивидуальный подход.</P>
                    
                    <div class="flex flex-wrap gap-x-7 gap-y-2">
                        <ButtonWhite class="relative z-10">Оставить заявку</ButtonWhite>
                        <ButtonBlue class="relative z-10 px-[59px]">Отзывы</ButtonBlue>
                    </div>

                </div>

                <div class="work_arrowsW"><img src="~/assets/img/work/arrows.png" alt="arrows" class="absolute bottom-7 right-14 z-0 work_arrows"></div>
            
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
<style lang="scss">
.work {
    background: linear-gradient(108.17deg, #3A97D1 0.88%, #01558B 100%);
    min-height: 455px;
}

.work__container {
    max-width: 1794px;
}
</style>