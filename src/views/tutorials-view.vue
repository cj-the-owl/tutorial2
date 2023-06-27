<template>
    <div v-if="tutorials" class="flex-container">
        <card-comp v-for="tutorial of tutorials" :key="tutorial.id" :tutorial="tutorial"/>
    </div>
    <div v-else>Loading...</div>
</template>

<script>
    import cardComp from '@/components/card-comp.vue';

    export default {
        computed: {
            tutorials() {
                return this.$store.state.tutorials
            }
        },
        mounted() {
            this.$store.dispatch("getTutorials")
        },

        components: {cardComp}
    }
</script>

<style>

</style>