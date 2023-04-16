<template>
    <footer class="footer min-h-[455px]">
        <div class="footer__container _container">
            <div class="footer__body max-w-[1075px] sm:flex justify-between items-center mt-[130px] mb-[40px] md:mb-[83px]">

                <div class="max-w-[256px] mb-[30px] md:mb-0">
                    <div class="footer__logoW"><img src="~/assets/img/footer/logo.png" alt="logo"
                            class="footer__logo mb-[18px]">
                    </div>
                    <P class="text-white">Привлечение поддержки и составление бизнес-планов.</P>
                </div>

                <div class="flex flex-wrap footer__contacts gap-x-[138px] gap-y-[20px] lg:gap-y-[60px]">

                    <div class="flex flex-col gap-y-[20px] lg:gap-y-[60px]">

                        <div class="flex flex-col gap-y-3">
                            <PContactsText>Мой телефон</PContactsText>
                            <PContactsBold ContactsLink="tel:+7 (123) 456-78-90">+7 (123) 456-78-90</PContactsBold>
                        </div>

                        <div class="flex flex-col gap-y-3">
                            <PContactsText>Telegram</PContactsText>
                            <PContactsBold ContactsLink="https://tg.me/name_account">@name_account</PContactsBold>
                        </div>
                    </div>

                    <div class="flex flex-col gap-y-3">
                        <PContactsText>Почта</PContactsText>
                        <PContactsBold ContactsLink="mailto:asdfgh@gmail.com">asdfgh@gmail.com</PContactsBold>
                    </div>


                </div>



            </div>

            <div class="footer__linkW flex justify-center mb-3">
                <a href="#" class="footer__link my-0 mx-auto">Политика обработки персональных данных</a>
            </div>

        </div>
    </footer>
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
.footer {
    background: linear-gradient(108.17deg, #3A97D1 0.88%, #01558B 100%);
}
</style>