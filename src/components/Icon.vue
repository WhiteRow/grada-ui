<template>
    <svg xmlns="http://www.w3.org/2000/svg"
        class="icon"
        :class="classes"
        :width="width"
        :height="height"
        :viewBox="viewBox"
        :aria-labelledby="iconName"
    >
        <title :id="iconName" lang="en">{{ iconName }} icon</title>

        <g :fill="iconColor">
            <slot />
        </g>
    </svg>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Icon',

        props: {
            iconName: {
                type: String,
                required: true,
            },

            viewBox: {
                type: String,
                required: true,
            },

            width: {
                type: [Number, String],
                default: 24,
            },

            height: {
                type: [Number, String],
                default: 24,
            },

            iconColor: {
                type: String,
                default: 'currentColor'
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
