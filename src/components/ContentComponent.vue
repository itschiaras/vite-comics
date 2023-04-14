<template>
    <div class="jumbo">
        <button class="text-uppercase border-0 cSeries">current series</button>
    </div>
    <div class="bg-dark">
        <div class="contentContainer container ">
            <div class="row row-cols-1 row-cols-sm-3 row-cols-md-6">
                <CardComponent v-for="(card, index) in cards" :key="index" :image="card.thumb" :title="card.series"/>
                <div class="w-100 d-flex justify-content-center">
                    <button class="text-uppercase border-0">load more</button>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
import CardComponent from './CardComponent.vue';
import { cards } from '../data/data.js';
export default {
    name: 'ContentComponent',
    components: { CardComponent },
    data() {
        return {
            cards: [...cards]
        }
    }
}
</script>

<style lang="scss" scoped>
    .jumbo {
        width: 100%;
        height: 400px;
        background-image: url(../assets/images/jumbotron.jpg);
        background-size: cover;
        position: relative;
    }

    button {
        background-color: #0282f9;
        color: white;
        font-weight: 700;
        padding: .5rem 3rem;
        margin-bottom: 1rem;
    }

    .cSeries {
        position: absolute;
        bottom: -20px;
        margin-bottom: 0;
        left: 100px;
        font-size: 1.5rem;
    }
</style>