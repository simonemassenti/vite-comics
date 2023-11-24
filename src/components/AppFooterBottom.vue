<script>
export default {
    data() {
        return {
            socials: [
                {
                    image: "facebook.png",
                    social: "Facebook",
                    link: ""
                },
                {
                    image: "twitter.png",
                    social: "Twitter",
                    link: ""
                },
                {
                    image: "youtube.png",
                    social: "YouTube",
                    link: ""
                },
                {
                    image: "pinterest.png",
                    social: "Pinterest",
                    link: ""
                },
                {
                    image: "periscope.png",
                    social: "Periscope",
                    link: ""
                }
            ]
        }
    },
        methods: {
            getImagePath(img) {
                return new URL(`../assets/img/footer-${img}`, import.meta.url).href;
            }
        }
}
</script>

<template>
    <div class="wrap">
        <div class="container">
            <a class="signup" href="">SIGN-UP NOW!</a>

            <div>
                <h3>FOLLOW US</h3>

                <ul>
                    <li v-for="social in socials">
                        <a href=""><img :src="getImagePath(social.image)" :alt="social.social"></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;
@use "../style/partials/_mixins" as *;

.wrap {
    background-color: $footer_color;
    .container {
    @include flex(row, space-between);
    height: 5rem;
    

    .signup {
        border: 2px solid $primary_color;
        padding: .5rem;
        color: $primary_color_text;
    }

    div {
        @include flex();
        h3 {
            color: $primary_color;
            margin-right: 1rem
        }

        ul {
            @include flex();
            
            li{
                margin-right: .5rem;
                width: 30px;
                a {
                    img {
                        width: 100%;
                    }
                }
            }
        }
    }
}
}

</style>