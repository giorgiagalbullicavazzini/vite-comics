<script>
import SignUpButton from './SignUpButton.vue';
import Socials from './Socials.vue';

export default {
    data() {
        return {
        }
    },
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

<style scoped>
#footer-bottom {
    background-color: #303030;
}

.container {
    align-items: center;
    display: flex;
    height: 110px;
    justify-content: space-between;
}
</style>