<script>
import MainBottom from './MainBottom.vue';
import MainTop from './MainTop.vue';

export default {
    name: 'DCMain',
    components: {
        MainBottom,
        MainTop
    }
}
</script>

<template>
    <main>
        <MainTop></MainTop>
        <MainBottom></MainBottom>
    </main>
</template>