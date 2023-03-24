<script>
// Import all components
import Jumbotron from './Jumbotron.vue';
import Logo from './Logo.vue';
import Navbar from './Navbar.vue';

export default {
    name: 'DCHeader',
    components: {
        Jumbotron,
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
        <div class="jumbotron">
            <Jumbotron></Jumbotron>
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
        justify-content: space-between;
    }
}
</style>