<template>
    <button class="bg-[#0077B6] buttonBlue py-3 px-9 active:brightness-90">
        <a class="font-600" href="#">
            <slot></slot>
        </a>
    </button>
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
<style scoped lang="scss">
.buttonBlue {
    border: 1px solid #FFFFFF;
    border-radius: 6px;
}
</style>