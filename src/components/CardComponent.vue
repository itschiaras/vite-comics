<template>
    <div class="col  pt-5 pb-5">
        <div class="text-center">
            <img :src="image" :alt="title" class="img-fluid">
        </div>
        <h5 class="text-white text-center text-uppercase mt-2">{{ title }}</h5>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ['image', 'title']
}
</script>

<style lang="scss" scoped>
img {
    max-height: 250px;
}
</style>