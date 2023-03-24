<script>
// Import all components
import DCFooter from './components/footer/DCFooter.vue';
import DCHeader from './components/header/DCHeader.vue';
import DCMain from './components/main/DCMain.vue';

export default {
  name: 'DCComics',
  components: {
    DCFooter,
    DCHeader,
    DCMain
  }
}
</script>

<template>
  <!-- Header -->
  <DCHeader />
  <!-- // Header -->

  <!-- Main -->
  <DCMain />
  <!-- // Main -->

  <!-- Footer -->
  <DCFooter />
  <!-- // Footer -->
</template>