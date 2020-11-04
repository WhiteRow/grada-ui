<template>
    <div class="page__wrapper">
        <div class="header">
            <div class="menu">
                <router-link to="/" class="menu__item">Home</router-link>
                <span class="menu__split">|</span>
                <router-link to="/gui" class="menu__item">Gui</router-link>
            </div>
        </div>
        <router-view />
    </div>
</template>

<style lang="scss">
    .header {
        padding: 40px 0;

        background-color:#30363d;
    }

    .menu {
        text-align: center;

        &__item {
            color: #FFFFFF;
        }

        &__split {
            margin-right: 10px;
            margin-left: 10px;

            color: #FFFFFF;
        }
    }
</style>

<script>
    export default {
        name: 'App',
    };
</script>
