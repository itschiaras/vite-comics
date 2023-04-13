<template>
    <main class="d-flex align-items-center">
        <div class="container ps-5 pe-5">
            <ul class="d-flex justify-content-between text-uppercase mb-0">
                <li v-for="(link, index) in mainLinks" :key="index">
                    <img class="img-fluid" src="" alt="">
                    <span>{{ link.description }}</span>
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
    }

}
</script>

<style lang="scss" scoped>
main {
    background-color: #0282f9;
    color: white;
    height: 100px;
}
</style>