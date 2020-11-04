<template>
    <div class="gui__container container">
        <h2 class="gui__title">Типографика</h2>

        <div class="gui__block">
            <h3 class="gui__title gui__title--sub">Заголовки без классов</h3>

            <h1>
                Заголовок первого уровня
            </h1>

            <h2>
                Заголовок второго уровня
            </h2>

            <h3>
                Заголовок третьего уровня
            </h3>

            <h4>
                Заголовок четвертого уровня
            </h4>
        </div>
        <!-- /.gui__block -->

        <div class="gui__block">
            <h3 class="gui__title gui__title--sub">Текст без класса</h3>

            <p>
                Учитывая ключевые сценарии поведения, понимание сути ресурсосберегающих технологий
                требует определения и уточнения распределения внутренних резервов и ресурсов.
                Следует отметить, что укрепление и развитие внутренней структуры выявляет срочную
                потребность вывода текущих активов. Значимость этих проблем настолько очевидна, что
                граница обучения кадров создаёт предпосылки для поставленных обществом задач.
            </p>
        </div>
        <!-- /.gui__block -->

        <div class="gui__block">
            <h3 class="gui__title gui__title--sub">Заголовки c классом</h3>

            <Heading tag="h1" :variations="['huge', 'section']">
                Заголовок первого уровня
            </Heading>

            <Heading tag="h2" :variations="['large', 'section']">
                Заголовок второго уровня
            </Heading>

            <Heading tag="h3" :variations="['big', 'block']">
                Заголовок третьего уровня
            </Heading>

            <Heading tag="h4">
                Заголовок четвертого уровня
            </Heading>
        </div>
        <!-- /.gui__block -->
    </div>
    <!-- /.gui__container container -->
</template>

<script lang="ts">
    import Vue from 'vue';
    import Heading from '../../components/Heading.vue';

    export default Vue.extend({
        name: 'GuiHeadings',

        components: {
            Heading,
        },
    });
</script>

<style lang="scss" scoped></style>
