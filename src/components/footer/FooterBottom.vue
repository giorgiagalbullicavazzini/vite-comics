<script>
import SignUpButton from './SignUpButton.vue';
import Socials from './Socials.vue';

export default {
    name: 'FooterBottom',
    components: {
        SignUpButton,
        Socials
    }
}
</script>

<template>
    <div id="footer-bottom">
        <div class="container">
            <SignUpButton></SignUpButton>
            <Socials></Socials>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

#footer-bottom {
    background-color: variables.$dark-color;

    .container {
        align-items: center;
        display: flex;
        justify-content: space-between;
        padding: 2.5rem 0;
    }
}
</style>