<template>
    <div class="cardsContainer container">
        <h3>Students are viewing</h3>
        <div class="cards">
            <div v-for="(data, i) in data" :key="i" class="card">
                <Card
                    :title="data.title"
                    :author="data.author"
                    :rating="data.rating"
                    :img="data.img"
                    :price="data.price"
                    :nb="data.nb"
                    :discount="data.discount"
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
                    title:
                        'Machine Learning A-Z™: Hands-On Python & R In Data Science',
                    rating: 4.0,
                    nb: 21232,
                    price: 20,
                    discount: 10,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title: 'AWS Certified Solutions Architect - Associate 2019',
                    rating: 4.0,
                    nb: 292301,
                    price: 20,
                    discount: 10,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title:
                        'The Complete JavaScript Course 2019: Build Real Projects!',
                    rating: 4.0,
                    nb: 212367,
                    price: 20,
                    discount: 10,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title:
                        'React - The Complete Guide (incl Hooks, React Router, Redux)',
                    rating: 4.0,
                    nb: 21292,
                    price: 20,
                    discount: 10,
                    img:
                        'https://images.unsplash.com/photo-1510519138101-570d1dca3d66?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80'
                },
                {
                    author: 'Stephen Grider',
                    title:
                        'Python for Data Science and Machine Learning Bootcamp',
                    nb: 21938,
                    rating: 4.0,
                    price: 20,
                    discount: 10,
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
    display: inline-block;
}

h3 {
    opacity: 0.7;
    font-size: 22px;
    margin-left: 10px;
    font-weight: 400;
    margin-bottom: 10px;
}
</style>
