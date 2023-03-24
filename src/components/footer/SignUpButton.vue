<script>
export default {
    name: 'SignUpButton',
}
</script>

<template>
    <a href="#">
        <button>Sign-up now!</button>
    </a>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

button {
    background-color: transparent;
    border: .125rem solid variables.$brand-color;
    color: variables.$main-color;
    cursor: pointer;
    font-family: inherit;
    font-size: inherit;
    padding: .625rem;
    text-transform: uppercase;
}
</style>