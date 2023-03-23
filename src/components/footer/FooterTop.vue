<script>
import FooterList from './FooterList.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        FooterList
    }
}
</script>

<template>
    <div id="footer-top">
        <div class="container">
            <div class="left column">
                <FooterList></FooterList>
                <FooterList></FooterList>
            </div>
            <div class="center column">
                <FooterList></FooterList>
            </div>
            <div class="right column">
                <FooterList></FooterList>
            </div>
        </div>
    </div>
</template>

<style scoped>
#footer-top {
    background-color: #1c1c1c;
}

.container {
    display: flex;
    height: 370px;
}

.column {
    margin: 30px 20px 30px 0;
}
</style>