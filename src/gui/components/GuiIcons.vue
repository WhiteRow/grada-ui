<template>
    <div class="gui__container container">
        <h2 class="gui__title">Иконки</h2>

        <div class="gui__block">
            <Icon name="test" />
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    import Vue from 'vue';
    import Icon from '../../components/Icon.vue';

    export default {
        name: 'GuiIcons',

        components: {
            Icon,
        },
    };
</script>

<style lang="scss"></style>
