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

            <div class="text-xs-left rating">
                <v-rating 
                    class="rate" 
                    small 
                    color="#f4c150"
                    background-color="#dedfe0"
                    dense
                    readonly
                    empty-icon="$vuetify.icons.ratingFull"
                    v-model="rating">
                </v-rating>
            </div>
            <div class="ratingNumber"> {{ rating }}</div>
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
        img: String,
        nb: Number
    }
};
</script>

<style scoped>
.customCard {
    font-size: 14px;
    box-shadow: 0px 1px 6px #e3e3e4;
    transition: 0.2s;
}
.customCard:hover {
    cursor: pointer;
    box-shadow: 0px 6px 10px #e3e3e4;
}

.rating {
    font-size: 14px;
}

img {
    height: 130px;
}

.rating {
    display: inline-block;
}

.ratingNumber {
    display: inline-block;
    position: relative;
    bottom: 1px;
    margin-left: 4px;
    font-size: 12px;
    font-weight: bold;
    opacity: .7;
}
</style>
