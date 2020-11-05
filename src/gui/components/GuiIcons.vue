<template>
    <div class="gui__container container">
        <h2 class="gui__title">Иконки</h2>

        <div class="gui__block">
            <Icon
                :variations="['user']"
                viewBox="0 0 456.368 456.368"
                iconName="user">
                    <IconUser />
            </Icon>
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    import Vue from 'vue';
    import Icon from '../../components/Icon.vue';
    import IconUser from '../../assets/icons/components/User.vue';

    export default Vue.extend({
        name: 'GuiIcons',

        components: {
            Icon,
            IconUser,
        },
    })
</script>

<style lang="scss"></style>
