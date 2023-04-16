<template>
    <section class="face">
        <div class="face__container _container">
            <div class="flex flex-col face__body justify-center mb-[58px]">

                <div class="flex justify-center flex-wrap  gap-x-[115px] gap-y-3 mt-[113px] mb-[62px]">
                    <div class="face__imgW"><img src="~/assets/img/face/face.png" alt="face" class="face__img"></div>
                    <div class="max-w-[540px]">
                        <H2 class="max-w-[485px] mb-4">Я помогу предпринимателям привлечь финансирование в бизнес</H2>
                        <P>Меня зовут Иванов Иван.<br>
                            <b>Моя основная деятельность</b> — это привлечение государственной поддержки. Помимо этого я
                            занимаюсь
                            составлением бизнес-планов и работой с частными фондами.
                        </P>
                    </div>
                </div>
            </div>
        </div>
    </section>


    <section class="face">
        <div class="face__greyTicketContainer">
            <div class="flex flex-col face__body justify-center">
                <GreyTicketCar class="max-w-[442px]"></GreyTicketCar>
            </div>
        </div>
    </section>

    <section class="face">
        <div class="face__container _container">
            <div class="flex flex-col face__body justify-center">

                <div class="flex justify-center mb-[59px]">
                    <FaceCarousel></FaceCarousel>
                </div>


                <div class="flex justify-center">
                    <ButtonBlue class="max-w-[230px]">Стать клиентом</ButtonBlue>
                </div>
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
.face__greyTicketContainer {
    max-width: 100%;
    margin: 0 auto;
    padding: 0px 15px 0px 0px;
    box-sizing: content-box;
}
</style>