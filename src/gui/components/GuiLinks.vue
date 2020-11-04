<template>
    <div class="gui__container container">
        <h2 class="gui__title">Ссылки</h2>

        <div class="gui__block">
            <a href="#">Ссылка без класса</a>
            <Exile path="#">Ссылка с классом</Exile>
            <Exile path="#" :variations="['with-icon', 'with-icon--left']">
                <div class="link__icon">icon</div>
                <span class="link__label">Ссылка с иконкой cлева</span>
            </Exile>
            <Exile path="#" :variations="['with-icon', 'with-icon--right']">
                <span class="link__label">Ссылка с иконкой справа</span>
                <div class="link__icon">icon</div>
            </Exile>
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    import Vue from 'vue';
    import Exile from '../../components/Exile.vue';

    export default {
        name: 'GuiLinks',

        components: {
            Exile,
        },
    };
</script>

<style lang="scss">
    a {
        &:not(:last-child) {
            margin-right: 10px;
        }
    }
</style>
