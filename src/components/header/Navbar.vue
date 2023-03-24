<script>
export default {
    data() {
        return {
            navbar: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Collectibles",
                "Videos",
                "Fans",
                "News",
                "Shop"
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
    text-transform: uppercase;
}

li {
    margin-left: 20px;
}
</style>