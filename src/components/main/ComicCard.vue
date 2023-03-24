<script>
export default {
    name: 'ComicCard',
    props: {
        img: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <div class="image">
            <img :src="img" :alt="title">
        </div>
        <h3>{{ title }}</h3>
    </div>
</template>

<style scoped>
.image {
    aspect-ratio: 1;
    width: 100%;
}
</style>