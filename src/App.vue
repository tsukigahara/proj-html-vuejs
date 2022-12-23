<script>

// import components
import AppHeader from './components/AppHeader.vue'
import AppHome from './components/AppHome.vue'
import AppAbout from './components/AppAbout.vue'
import AppServices from './components/AppServices.vue'
import AppProcess from './components/AppProcess.vue'
import AppTeam from './components/AppTeam.vue'
import AppNews from './components/AppNews.vue'
import AppKnow from './components/AppKnow.vue'
import AppFooter from './components/AppFooter.vue'

// import json
import links from './assets/links.json'


export default {
    data() {
        return {
            links,
        }
    },
    components: {
        AppHeader,
        AppHome,
        AppAbout,
        AppServices,
        AppProcess,
        AppTeam,
        AppNews,
        AppKnow,
        AppFooter
    }
}
</script>

<template>
    <AppHeader :list="links" />
    <AppHome />
    <AppAbout />
    <AppServices />
    <AppProcess />
    <AppTeam />
    <AppNews />
    <AppKnow />
    <AppFooter :list="links" />
</template>

<style lang="scss" scoped>
@use './styles/general.scss' as *;
@use './styles/partial/variables' as *;
</style>
