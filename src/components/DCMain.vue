<script>
import MainBottom from './MainBottom.vue';
import MainTop from './MainTop.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        MainBottom,
        MainTop
    }
}
</script>

<template>
    <div id="main">
        <MainTop></MainTop>
        <MainBottom></MainBottom>
    </div>
</template>