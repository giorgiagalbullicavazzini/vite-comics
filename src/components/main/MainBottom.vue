<script>
export default {
    data() {
        return {
            buttons: [
                "digital comics",
                "dc merchandise",
                "subscription",
                "comic shop locator",
                "dc power visa"
            ]
        }
    }
}
</script>

<template>
    <div id="main-bottom">
        <div class="container">
            <div v-for="button in buttons" class="button">
                <div class="image"></div>
                <div class="text">{{ button }}</div>
            </div>
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

.button {
    align-items: center;
    color: #ffffff;
    display: flex;
    margin: 0 20px;
}

.image {
    aspect-ratio: 1;
    background-color: #ffffff;
    margin-right: 10px;
    width: 50px;
}
</style>