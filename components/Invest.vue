<template>
    <div class="relative min-h-[1290px] invest__outer">
        <section class="invest">
            <div class="invest__container _container">
                <div class="invest__body">

                    <div class="md:flex gap-x-[67px]">

                        <div>
                            <div class="dotsW"><img src="~/assets/img/invest/dots.svg" alt="dots"
                                    class="absolute top-[31px] left-[18px] dots"></div>
                            <GreyTicket class="mb-8"></GreyTicket>
                            <P class="mb-10 max-w-[372px]">Привлечение государственной поддержки и составление бизнес-планов
                            </P>
                            <ButtonBlue class="px-[59px] mb-[10px] md:mb-0">Начать</ButtonBlue>
                        </div>

                        <div class="grey__imgW"><img src="~/assets/img/invest/grey.jpg" alt="grey image"
                                class="max-w-[150%] grey__img"></div>

                        <div class="dotsW"><img src="~/assets/img/invest/dots.svg" alt="dots"
                                class="absolute top-[755px] right-[62px] dots"></div>
                    </div>

                    <div class="invest__cards flex flex-wrap justify-center max-w-[1286px] gap-x-[72px] gap-y-5">
                        <InvestCard ImageSrc="img/cards/01.svg" ImageAlt="01" Subtitle="Привлечение финансирования"
                            Paragraph="Рассказываем бизнесу о методах привлечения финансирования">
                        </InvestCard>
                        <InvestCard ImageSrc="img/cards/02.svg" ImageAlt="02" Subtitle="Составление бизнес планов"
                            Paragraph="Мировые стандарты оформления финансового планирования и гарантия">
                        </InvestCard>
                        <InvestCard ImageSrc="img/cards/03.svg" ImageAlt="03" Subtitle="Государственные программы"
                            Paragraph="Актуальный перечень направлений государственной поддержки">
                        </InvestCard>
                    </div>
                </div>
            </div>
        </section>
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
    },
    methods: {
    }
}
</script>

<!-- component style -->
<style lang="scss">
.invest__cards {
    margin: 0 auto;
}
.invest__outer {
    background: rgba(21, 108, 164, 0.02);
}
</style>