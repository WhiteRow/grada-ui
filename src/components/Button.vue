<template>
    <button class="button" :class="classes">

    </button>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Button',

        props: {
            variations: {
                type: Array,
                default: () => [],
            },
        },

        computed: {
            classes() {
                return this.variations.map(variation => {
                    return `icon--${variation}`;
                });
            },
        },
    });
</script>
