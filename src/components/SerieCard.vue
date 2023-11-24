<script>
export default {
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <div>
            <img :src="image" :alt="title">
        </div>

        <p>{{ title }}</p>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *; 
.card {
    margin: .5rem;

    div {
        height: 100px;
        overflow: hidden;
        margin-bottom: .5rem;
        text-align: center;
        img {
            width: 100%;
        }
    }

    p {
        color: $primary_color_text;
        font-size: .8rem;
    }

    

}
</style>