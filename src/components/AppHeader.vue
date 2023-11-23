<script>
export default {
    data() {
        return {
            navMenu : [
                {
                    title: "Characters",
                    status: false
                },
                {
                    title: "Comics",
                    status: true
                },
                {
                    title: "Movies",
                    status: false
                },
                {
                    title: "Tv",
                    status: false
                },
                {
                    title: "Games",
                    status: false
                },
                {
                    title: "Collectibles",
                    status: false
                },
                {
                    title: "Videos",
                    status: false
                },
                {
                    title: "Fans",
                    status: false
                },
                {
                    title: "News",
                    status: false
                },
                {
                    title: "Shop",
                    status: false
                }
            ]
        }
    }
}
</script>

<template>
<header>
    <img src="../assets/img/dc-logo.png" alt="">
    
    <ul class="menu">
        <li v-for="item in navMenu" :class="{'active': item.status}">{{ item.title.toUpperCase() }}</li>
    </ul>
</header>
</template>

<style lang="scss" scoped>
@use "../style/partials/header";
</style>