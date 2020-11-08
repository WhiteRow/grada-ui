<template>
    <button
        class="button"
        :class="classes"

    >
        <slot />
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
                    return `button--${variation}`;
                });
            },
        },
    });
</script>
