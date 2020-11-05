<template>
    <div class="gui__container container">
        <h2 class="gui__title">Кнопки</h2>

        <div class="gui__block">
            <Button />
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    import Vue from 'vue';
    import Button from '../../components/Button.vue';

    export default Vue.extend({
        name: 'GuiButtons',

        components: {
            Button
        }
    })
</script>

<style>

</style>