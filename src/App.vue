<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue';
import AppMain from './components/AppMain.vue';
import AppFooterTop from'./components/AppFooterTop.vue';
import AppFooterBottom from'./components/AppFooterBottom.vue';
export default {
    components: {
        AppHeader,
        AppHero,
        AppMain,
        AppFooterTop,
        AppFooterBottom
    },
    data () {
        return {

        }
    }
}
</script>

<template>
<AppHeader />
<AppHero />
<AppMain />
<AppFooterTop />
<AppFooterBottom />
</template>

<style>

</style>
