<template>
    <div class="gui__container container">
        <h2 class="gui__title">Списки</h2>

        <div class="gui__block">
            <h3 class="gui__title gui__title--sub">Список без класса</h3>

            <ul>
                <li>Пункт списка 1</li>
                <li>Пункт списка 2</li>
                <li>Пункт списка 3</li>
                <li>Пункт списка 4</li>
                <li>Пункт списка 5</li>
            </ul>
        </div>
        <!-- /.gui__block -->

        <div class="gui__block">
            <h3 class="gui__title gui__title--sub">Списки с классом</h3>

            <ul class="list list--reseted">
                <li>Пункт списка 1</li>
                <li>Пункт списка 2</li>
                <li>Пункт списка 3</li>
                <li>Пункт списка 4</li>
                <li>Пункт списка 5</li>
            </ul>
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    export default {
        name: 'GuiLists',
    };
</script>

<style lang="scss"></style>
