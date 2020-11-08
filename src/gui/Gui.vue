<template>
    <div class="gui__wrapper">
        <div class="gui__block container">
            <h1 class="gui__title gui__title--main">
                <span class="gui__highlight">Grada</span>
                Gui.
            </h1>
        </div>

        <GuiTypography />

        <GuiIcons />

        <GuiLinks />

        <GuiButtons />

        <GuiLists />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    import GuiTypography from './components/GuiTypography.vue';
    import GuiIcons from './components/GuiIcons.vue';
    import GuiLinks from './components/GuiLinks.vue';
    import GuiButtons from './components/GuiButtons.vue';
    import GuiLists from './components/GuiLists.vue';

    export default Vue.extend({
        name: 'Gui',
        components: {
            GuiTypography,
            GuiIcons,
            GuiLinks,
            GuiButtons,
            GuiLists,
        },
    });
</script>

<style lang="scss">
    .gui {
        &__wrapper {
            margin-top: 50px;

            & .button {
                margin-bottom: 20px;

                &:not(:last-child) {
                    margin-right: 20px;
                }
            }
        }

        &__container {
            &.container {
                margin-bottom: 80px;
            }
        }

        &__block {
            margin-top: 60px;

            &--centered {
                display: flex;
                align-items: center;
                flex-wrap: wrap;
            }
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
