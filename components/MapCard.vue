<template>
    <div class="flex flex-col w-full sm:w-1/3 sm:max-w-[300px] ">
        <P class="font-semibold mb-[15px] text-[#363636]">{{ Subtitle }}</P>
        <P class="font-normal text-[#363636]">{{ Paragraph }}</P>
    </div>
</template>


<!-- component script -->
<script>
export default {
    /* passed props */
    props: {
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

<!-- component style -->
<style lang="scss"></style>