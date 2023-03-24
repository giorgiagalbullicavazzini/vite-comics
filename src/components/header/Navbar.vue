<script>
export default {
    name: 'Navbar',
    data() {
        return {
            navbar: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop'
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

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

ul {
    display: flex;
    text-transform: uppercase;

    li {
        margin-left: 1.25rem;

        a {
            color: variables.$darken-color;

            &.active {
                border-bottom: 5px solid variables.$brand-color;
                color: variables.$brand-color;
            }
        }
    }
}
</style>