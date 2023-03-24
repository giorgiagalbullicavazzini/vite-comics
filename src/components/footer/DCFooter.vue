<script>
import FooterBottom from './FooterBottom.vue';
import FooterTop from './FooterTop.vue';

export default {
    name: 'DCFooter',
    components: {
        FooterBottom,
        FooterTop
    }
}
</script>

<template>
    <footer>
        <FooterTop></FooterTop>
        <FooterBottom></FooterBottom>
    </footer>
</template>