<script>
export default {
    name: 'Navbar',
    data() {
        return {
            navbar: [
                {
                    item: 'Characters',
                    active: true,
                },
                {
                    item: 'Comics',
                    active: false,
                },
                {
                    item: 'Movies',
                    active: false,
                },
                {
                    item: 'TV',
                    active: false,
                },
                {
                    item: 'Games',
                    active: false,
                },
                {
                    item: 'Collectibles',
                    active: false,
                },
                {
                    item: 'Videos',
                    active: false,
                },
                {
                    item: 'Fans',
                    active: false,
                },
                {
                    item: 'News',
                    active: false,
                },
                {
                    item: 'Shop',
                    active: false,
                }
            ]
        }
    }
}
</script>

<template>
    <div id="navbar">
        <ul>
            <li v-for="item in navbar"><a href="#" :class="{ active: item.active === true }">{{ item.item }}</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

ul {
    align-items: center;
    display: flex;
    text-transform: uppercase;

    li {
        margin-left: 1.875rem;

        a {
            border-bottom: variables.$navbar-border solid transparent;
            color: variables.$darken-color;
            display: inline-block;
            font-weight: 600;
            line-height: 7.5rem;

            &.active,
            &:hover {
                border-bottom: variables.$navbar-border solid variables.$brand-color;
                color: variables.$brand-color;
            }
        }
    }
}
</style>