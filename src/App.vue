<template>
    <main>
        <nav-header />
        <router-view />
        <game-modal />
        <search-modal />
    </main>
</template>

<script>
import GameModal from '@/components/GameModal/GameModal';
import SearchModal from '@/components/SearchModal/SearchModal';
import NavHeader from '@/components/NavHeader/NavHeader';

export default {
    name: 'App',

    components: {
        NavHeader,
        GameModal,
        SearchModal,
    },
};
</script>

<style lang="scss" rel="stylesheet/scss">
    @import "~styles/variables.scss";
    @import url('https://fonts.googleapis.com/css?family=Roboto:400,700');

    body {
        font-family: 'Roboto', sans-serif;
    }

    .at-loading-bar__inner {
        background-color: $nin-white !important;
    }
</style>
