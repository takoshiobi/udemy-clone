<template>
    <div class="cardsContainer container-fluid">
        <h3>Students are viewing</h3>
        <div class="row cards">
            <div v-for="(data, i) in data" :key="i" class="card">
                <Card
                    :title="data.title"
                    :author="data.author"
                    :rating="data.rating"
                    :img="data.img"
                    :price="data.price"
                    :nb="nb"
                />
            </div>
        </div>
    </div>
</template>

<script>
import Card from './Card.vue';

export default {
    components: {
        Card
    },
    data() {
        return {
            data: [
                {
                    author: 'Stephen Grider',
                    title: 'Python for Data Science and ML',
                    rating: 4.7,
                    nb: 2123,
                    price: 20,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title: 'Python for Data Science and ML',
                    rating: 4.4,
                    nb: 2923,
                    price: 20,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title: 'Python for Data Science and ML',
                    rating: 4.8,
                    nb: 2123,
                    price: 20,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title: 'Python for Data Science and ML',
                    rating: 4.6,
                    nb: 2129,
                    price: 20,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title: 'Python for Data Science and ML',
                    nb: 2193,
                    rating: 4.2,
                    price: 20,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                }
            ]
        };
    }
};
</script>

<style scoped>
.cards {
    width: 100%;
    margin: 0 auto;
}

.card {
    margin: 0 4px;
    border: none !important;
}

h3 {
    opacity: 0.7;
    font-size: 22px;
    margin-left: 10px;
    font-weight: 400;
    margin-bottom: 10px;
}
</style>
