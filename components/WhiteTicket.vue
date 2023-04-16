<template>
    <div class="relative z-10 mb-[18px] text-white">
        <div class="flex items-center gap-x-4">
            <div class=" whiteLine min-w-[48px] h-0 mt-[31px]"></div>
            <P class="mt-[31px] text-white">Вы больше чем клиент</P>
        </div>
        <H1 class="text-[48px] leading-[51px] mt-[14px] text-white">Работа с клиентами</H1>
    </div>
</template>


<!-- component script -->
<script>
export default {
    /* passed props */
    props: {
        Subtitle: String,
        Text: String,
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
.whiteLine {
    border: 1px solid white;
}
</style>