<template>
    <div class="relative z-10 outerGreyTicket bg-gray-200 mb-[70px]">
        <div class="flex items-center gap-x-4">
            <div class=" blueLine min-w-[48px] h-0 mt-[31px]"></div>
            <P class="mt-[31px]">Основная часть наших клиентов -
                это производственные предприятия.</P>
        </div>
        <H1 class="mt-[14px] pb-7 !text-[42px]">Партнеры</H1>
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
.blueLine {
    border: 1px solid #0077B6;
}
</style>