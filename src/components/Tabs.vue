<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-md-5 col-lg-5 col-lx-5 recContainer">
                <div class="rec">
                    <h4>The world’s largest selection of courses</h4>
                    <p>
                        Choose from over 100,000 online video courses with new
                        additions published every month
                    </p>
                </div>
            </div>
            <div class="col-12 col-md-7 col-lg-7 col-lx-7 tabs">
                <div class="tabContainer">
                    <v-tabs
                        v-model="active"
                        color="transparent"
                        slider-color="#007791"
                    >
                        <v-tab ripple> Development </v-tab>
                        <v-tab ripple> Design </v-tab>
                        <v-tab ripple> Marketing </v-tab>
                        <v-tab ripple> Business </v-tab>
                        <v-tab ripple> IT & Software </v-tab>
                        <v-tab ripple> Personal Development </v-tab>
                        <v-tab ripple> Marketing </v-tab>
                        <v-tab ripple> Photography </v-tab>
                        <v-tab-item v-for="n in 7" :key="n">
                            <v-card flat>
                                <div class="cardContainer">
                                    <div
                                        v-for="(data, i) in data"
                                        :key="i"
                                        class="card"
                                    >
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
                            </v-card>
                        </v-tab-item>
                    </v-tabs>
                </div>
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
            active: null,
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
                        'https://images.unsplash.com/photo-1526374965328-7f61d4dc18c5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80'
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
                        'https://images.unsplash.com/photo-1480694313141-fce5e697ee25?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=750&q=80'
                }
            ]
        };
    },
    methods: {
        next() {
            const active = parseInt(this.active);
            this.active = active < 2 ? active + 1 : 0;
        }
    }
};
</script>

<style scoped>
.tabs {
    padding: 0;
    margin: 0;
}

.rec {
    display: table;
    margin: 0 auto;
    height: 350px;
    padding: 0;
    background: #f7f8fa;
    position: relative;
    top: 20px;
}

.rec h4 {
    margin-top: 130px;
}

.rec h4,
.rec p {
    margin-left: 20px;
}

.rec p {
    font-size: 16px;
}

.card {
    display: inline-block;
    margin: 10px 3px;
    border: none !important;
}

@media (max-width: 1140px) {
    .recContainer {
        display: none;
    }

    .tabs {
        width: 80%;
        display: table;
        margin: 0 auto;
    }

    .cardContainer {
        margin-left: 12%;
    }
}

@media (max-width: 992px) {
    .recContainer {
        display: none;
    }

    .cardContainer {
        margin-left: 4%;
    }
}

@media (max-width: 768px) {
    .cardContainer {
        margin-left: 1%;
    }
}

@media (max-width: 576px) {
    .cardContainer {
        margin-left: 1%;
    }
}
</style>
