<script>
export default {
    data() {
        return {
            dcComics: [
                {
                    title: "Characters"
                },
                {
                    title: "Comics"
                },
                {
                    title: "Movies"
                },
                {
                    title: "TV"
                },
                {
                    title: "Games"
                },
                {
                    title: "Videos"
                },
                {
                    title: "News"
                }
            ],
            shop: [
                {
                    title: "Shop DC"
                },
                {
                    title: "Shop DC Collectables"
                }
            ],
            dc: [
                {
                    title: "Terms Of Use"
                },
                {
                    title: "Privacy policy (New)"
                },
                {
                    title: "Ad Choices"
                },
                {
                    title: "Advertising"
                },
                {
                    title: "Jobs"
                },
                {
                    title: "Subscriptions"
                },
                {
                    title: "Talent Workshops"
                },
                {
                    title: "CPSC Certificates"
                },
                {
                    title: "Ratings"
                },
                {
                    title: "Shop Help"
                },
                {
                    title: "Contact Us"
                }
            ],
            sites: [
                {
                    title: "DC"
                },
                {
                    title: "MAD Magazine"
                },
                {
                    title: "DC Kids"
                },
                {
                    title: "DC Universe"
                },
                {
                    title: "DC Power Visa"
                }
            ]
        }
    }
}
</script>

<template>
    <div class="footer-top">
        <div>
            <ul>
                <li class="title">DC COMICS</li>
                <li>
                    <ul>
                        <li v-for="item in dcComics" class="subtitle"> {{ item.title }} </li>
                    </ul>
                </li>
            </ul>

            <ul>
                <li class="title">SHOP</li>
                <li>
                    <ul>
                        <li v-for="item in shop" class="subtitle"> {{ item.title }} </li>
                    </ul>
                </li>
            </ul>
        </div>

        <div>
            <ul>
                <li class="title">DC</li>
                <li>
                    <ul>
                        <li v-for="item in dc" class="subtitle"> {{ item.title }} </li>
                    </ul>
                </li>
            </ul>
        </div>

        <div>
            <ul>
                <li class="title">SITES</li>
                <li>
                    <ul>
                        <li v-for="item in sites" class="subtitle"> {{ item.title }} </li>
                    </ul>
                </li>
            </ul>
        </div>

    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/footer-top";
</style>