<template>
    <svg class="icon" :name="name" :classes="classes">
        <use xlink:href="" />
    </svg>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Icon',

        props: {
            name: {
                type: String,
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
