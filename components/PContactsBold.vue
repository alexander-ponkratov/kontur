<template>
    <a :href="ContactsLink" class="font-semibold text-[16px] leading-[20px] text-white"><slot></slot></a>
</template>


<!-- component script -->
<script>
export default {
    /* passed props */
    props: {
        ContactsLink: String
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

</style>