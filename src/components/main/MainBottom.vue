<script>
import ShopButton from './ShopButton.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        ShopButton
    }
}
</script>

<template>
    <div id="main-bottom">
        <div class="container">
            <ShopButton></ShopButton>
            <ShopButton></ShopButton>
            <ShopButton></ShopButton>
            <ShopButton></ShopButton>
            <ShopButton></ShopButton>
        </div>
    </div>
</template>

<style scoped>
#main-bottom {
    background-color: #0282f9;
}

.container {
    align-items: center;
    display: flex;
    justify-content: center;
    height: 155px;
}
</style>