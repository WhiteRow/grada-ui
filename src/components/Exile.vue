<template>
    <a :href="path" class="link" :class="classes">
        <slot></slot>
    </a>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Exile',

        props: {
            path: {
                type: String,
                default: '/',
            },

            variations: {
                type: Array,
                default: () => [],
            },
        },

        computed: {
            classes() {
                return this.variations.map(variation => {
                    return `link--${variation}`;
                });
            },
        },
    });
</script>

<style></style>
