<script>
export default {
    data() {
        return {
            buyMenu: [
                {
                    name: "digital comics",
                    image: "comics-digital-comics.png"
                },
                {
                    name: "dc merchandise",
                    image: "comics-merchandise.png"
                },
                {
                    name: "subscription",
                    image: "comics-subscriptions.png"
                },
                {
                    name: "comic shop locator",
                    image: "comics-shop-locator.png"
                },
                {
                    name: "dc power visa",
                    image: "dc-power-visa.svg"
                }
            ]
        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/buy-${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="main">

        <div>
            <ul>
                <li v-for="item in buyMenu">
                    <img :src="getImagePath(item.image)" alt="">
                    <span>{{ item.name.toUpperCase() }}</span>
                </li>
            </ul>
        </div>

    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/main"
</style>