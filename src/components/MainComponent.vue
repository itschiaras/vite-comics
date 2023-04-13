<template>
    <main class="d-flex align-items-center">
        <div class="container ps-5 pe-5">
            <ul class="d-flex justify-content-between text-uppercase mb-0">
                <li v-for="(link, index) in mainLinks" :key="index" class="d-flex align-items-center">
                    <a href="">
                        <img :src="getImagePath(`../assets/images/${link.src}`)" alt="">
                        <span>{{ link.description }}</span>
                    </a>

                </li>
            </ul>
        </div>

    </main>
</template>

<script>
import { mainImg } from '../data/data.js';
export default {
    name: 'MainComponent',
    data() {
        return {
            mainLinks: mainImg
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }

}
</script>

<style lang="scss" scoped>
main {
    background-color: #0282f9;
    color: white;
    height: 100px;

    img {
        width: 40px;
        margin-right: 1rem;
    }

    a {
        text-decoration: none;
        color: white;
    }
}
</style>