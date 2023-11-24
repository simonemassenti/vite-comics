<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppCurrentSeries from './components/AppCurrentSeries.vue';
import AppMain from './components/AppMain.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';
export default {
    components: {
        AppHeader,
        AppJumbotron,
        AppCurrentSeries,
        AppMain,
        AppFooterTop,
        AppFooterBottom
    },
    data() {
        return {
        }
    }
}
</script>

<template>
    <AppHeader />
    <AppJumbotron/>
    <AppCurrentSeries/>
    <AppMain />
    <AppFooterTop />
    <AppFooterBottom />
</template>

<style lang="scss">
@use "./style/general.scss";
</style>
