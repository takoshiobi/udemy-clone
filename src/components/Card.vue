<template>
    <div>
        <b-card
            :title="title"
            :img-src="img"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 15rem;"
            class="customCard"
        >
            <b-card-text>
                {{ author }}
            </b-card-text>

            <div class="text-xs-left rating">
                <v-rating 
                    class="rate" 
                    color="#f4c150"
                    background-color="#dedfe0"
                    dense
                    readonly
                    size="14px"
                    empty-icon="$vuetify.icons.ratingFull"
                    v-model="rating"
                >
                </v-rating>
            </div>
            <div class="ratingNumber"> {{ rating }}</div>
            <div class="nbUsers"> ({{ String(nb).slice(0,-3) + "," + String(nb).slice(-3) }})</div>
            <div class="price">${{ price }}</div>
            <div class="discount">$10</div>
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
        nb: Number,
        discount: Number
    }
};
</script>

<style scoped>
.customCard { 
    box-shadow: 0px 1px 6px #e3e3e4;
    transition: 0.2s;
}
.customCard:hover {
    cursor: pointer;
    box-shadow: 0px 6px 10px #e3e3e4;
}

p {
    font-size: 12px;
    opacity: .7;
}

.rating {
    font-size: 12px;
    display: inline-block;
}

img {
    height: 130px;
}

h4 {
    font-size: 16px;
    opacity: .95;
   overflow: hidden;
   text-overflow: ellipsis;
   display: -webkit-box;
   -webkit-box-orient: vertical;
   -webkit-line-clamp: 2;
   line-height: 1.3em;        
   max-height: 2*2em; 
}

.ratingNumber {
    display: inline-block;
    position: relative;
    bottom: 1px;
    margin-left: 4px;
    font-size: 11px;
    font-weight: bold;
    opacity: .7;
}

.nbUsers {
    font-size: 11px;
    opacity: 0.7;
    display: inline-block;
    position: relative;
    bottom: 1px;
    margin-left: 4px;
}

.price {
    text-align: center;
    padding-top: 10px;
    opacity: .6;
    text-decoration: line-through;

}

.discount {
    position: absolute;
    right: 10px;
    bottom: 0;
    font-size: 20px;
}

div {
    padding-bottom: 6px;
}
</style>
