<template>
    <UnderConstruction />
</template>
<script>
import UnderConstruction from './Auxiliary/UnderConstruction.vue';

export default {
    name: "Home",
    components: {
        UnderConstruction,
    },
    data() {
        return {
            pageTitle: "Home",
        };
    },
    methods: {
        setPageTitle() {
            this.$store.dispatch("changePageTitle", this.pageTitle);
        },
    },
    mounted() {
        this.setPageTitle();
    },
}
</script>