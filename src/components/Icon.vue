<template>
    <component :is="tag" class="icon" :class="classes">
        <slot></slot>
    </component>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Icon',

        props: {
            tag: {
                type: String,
                default: 'svg',
            },

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

<style lang="scss"></style>
