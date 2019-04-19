<template>
    <div class="card">
        <b-card
            :title="title"
            :img-src="img"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 16rem;"
            class="mb-2 customCard"
        >
            <b-card-text>
                {{ author }}
            </b-card-text>

            <div class="text-xs-left">
                <v-rating class="rating" small v-model="rating"></v-rating>
            </div>
        </b-card>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        author: String,
        price: Number,
        rating: Number,
        img: String
    }
}
</script>

<style scoped>
    .customCard {
        font-size: 16px;
        box-shadow: 0px 1px 10px #e3e3e4;
        transition: .2s;
    }
    .customCard:hover {
        cursor: pointer;
        box-shadow: 10px 5px 10px #e3e3e4;
    }

    .rating {
        font-size: 14px;
    }
</style>


