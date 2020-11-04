<template>
    <div class="gui__wrapper">
        <div class="gui__block container">
            <h1 class="gui__title gui__title--main">
                <span class="gui__highlight">Grada</span>
                Gui.
            </h1>
        </div>

        <GuiTypography />

        <GuiLinks />

        <GuiLists />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    import GuiTypography from './components/GuiTypography.vue';
    import GuiLinks from './components/GuiLinks.vue';
    import GuiLists from './components/GuiLists.vue';

    export default Vue.extend({
        name: 'Gui',
        components: {
            GuiTypography,
            GuiLinks,
            GuiLists,
        },
    });
</script>

<style lang="scss">
    .gui {
        &__wrapper {
            margin-top: 50px;
        }

        &__container {
            &.container {
                margin-bottom: 80px;
            }
        }

        &__block {
            margin-top: 60px;
        }

        &__title {
            font-size: 44px;
            text-align: center;

            margin-bottom: 40px;

            &--main {
                font-size: 54px;
            }

            &--sub {
                font-size: 38px;
                text-align: left;
            }
        }

        &__highlight {
            color: #f27a54;
        }
    }
</style>
