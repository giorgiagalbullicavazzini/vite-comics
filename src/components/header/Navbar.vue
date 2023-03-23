<script>
export default {
    data() {
        return {
            navbar: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop"
            ]
        }
    }
}
</script>

<template>
    <div id="navbar">
        <ul>
            <li v-for="item in navbar"><a href="#">{{ item }}</a></li>
        </ul>
    </div>
</template>

<style scoped>
ul {
    display: flex;
    list-style: none;
}

li {
    margin-left: 20px;
}
</style>