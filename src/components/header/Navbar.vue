<script>
import NavbarItems from './NavbarItems.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        NavbarItems
    }
}
</script>

<template>
    <div id="navbar">
        <ul>
            <NavbarItems></NavbarItems>
            <NavbarItems></NavbarItems>
            <NavbarItems></NavbarItems>
            <NavbarItems></NavbarItems>
            <NavbarItems></NavbarItems>
        </ul>
    </div>
</template>

<style scoped>
ul {
    display: flex;
    list-style: none;
}
</style>