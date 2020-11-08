<template>
    <div class="gui__container container">
        <h2 class="gui__title">Кнопки</h2>

        <div class="gui__block gui__block--centered">
            <Button :variations="['simple', 'small']">
                <span class="button__label">Кнопка</span>
            </Button>

            <Button :variations="['filled', 'small']">
                <span class="button__label">Маленькая кнопка</span>
            </Button>

            <Button :variations="['unfilled', 'small']">
                <span class="button__label">Маленькая кнопка</span>
            </Button>

            <Button :variations="['unfilled', 'medium', 'iconed', 'icon-right']">
                <span class="button__label">Кнопка с икокной</span>

                <Icon
                    class="button__icon"
                    :variations="['user']"
                    viewBox="0 0 456.368 456.368"
                    iconName="user"
                    width="20px"
                    height="20px"
                >
                    <IconUser />
                </Icon>
            </Button>

            <Button :variations="['filled', 'medium', 'iconed', 'icon-left']">
                <Icon
                    class="button__icon"
                    :variations="['user']"
                    viewBox="0 0 456.368 456.368"
                    iconName="user"
                    width="20px"
                    height="20px"
                >
                    <IconUser />
                </Icon>

                <span class="button__label">Кнопка с икокной</span>
            </Button>

            <Button
                :variations="['filled', 'content', 'iconed', 'angle-right']"
                style="max-width: 270px"
            >
                <Icon
                    class="button__icon"
                    :variations="['user']"
                    viewBox="0 0 456.368 456.368"
                    iconName="user"
                    width="20px"
                    height="20px"
                >
                    <IconUser />
                </Icon>

                <span class="button__label">Кнопка контентная</span>
            </Button>

            <Button :variations="['icon', 'filled']">
                <Icon
                    class="button__icon"
                    :variations="['user']"
                    viewBox="0 0 456.368 456.368"
                    iconName="user"
                    width="14px"
                    height="14px"
                >
                    <IconUser />
                </Icon>
            </Button>
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    import Vue from 'vue';
    import Button from '../../components/Button.vue';
    import Icon from '../../components/Icon.vue';
    import IconUser from '../../assets/icons/components/User.vue';

    export default Vue.extend({
        name: 'GuiButtons',

        components: {
            Button,
            Icon,
            IconUser,
        },
    });
</script>

<style></style>
