<template>
    <component :is="tag" class="heading" :class="classes">
        <slot></slot>
    </component>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Heading',

        props: {
            tag: {
                type: String,
                default: 'h1',
            },

            variations: {
                type: Array,
                default: () => [],
            },
        },

        computed: {
            classes() {
                return this.variations.map(variation => {
                    return `heading--${variation}`;
                });
            },
        },
    });
</script>

<style lang="scss"></style>
