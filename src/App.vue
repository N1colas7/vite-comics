<script>
    import AppHeader from './components/AppHeader.vue';
    import AppContent from './components/AppContent.vue';
    import AppFooter from './components/AppFooter.vue';

    export default {
        components:{
            AppHeader,
            AppContent,
            AppHeader
        }
    }
</script>

<template lang="">
    <AppHeader />
</template>

<style lang="scss">
    @use './styles/generals.scss' as *;
    *{
        padding: 0;
        margin: 0 auto;
        box-sizing: border-box;
    }
</style>
