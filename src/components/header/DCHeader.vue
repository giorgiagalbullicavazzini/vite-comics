<script>
// Import all components
import Logo from './Logo.vue';
import Navbar from './Navbar.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        Logo,
        Navbar
    }
}
</script>

<template>
    <header>
        <div class="container">
            <Logo></Logo>
            <Navbar></Navbar>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

header {
    background-color: variables.$main-color;

    .container {
    align-items: center;
    display: flex;
    padding: 1.125rem 0;
    justify-content: space-between;
    }
}
</style>