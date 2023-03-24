<script>
export default {
    name: 'MainTop',
}
</script>

<template>
    <div id="main-top">
        <div class="container">
            --&gt; Content goes here &lt;--
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables';

#main-top {
    background-color: variables.$darken-color;

    .container {
        align-items: center;
        color: variables.$main-color;
        display: flex;
        font-size: 1.75rem;
        font-weight: 600;
        padding: 3.125rem 0;
    }
}
</style>