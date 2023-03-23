<script>
import FooterBottom from './FooterBottom.vue';
import FooterTop from './FooterTop.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        FooterBottom,
        FooterTop
    }
}
</script>

<template>
    <div id="footer">
        <FooterTop></FooterTop>
        <FooterBottom></FooterBottom>
    </div>
</template>