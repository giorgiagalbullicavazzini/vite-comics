<script>
// Import all components
import DCFooter from './components/DCFooter.vue';
import DCHeader from './components/DCHeader.vue';
import DCMain from './components/DCMain.vue';

export default {
  components: {
    DCFooter,
    DCHeader,
    DCMain
  }
}
</script>

<template>
  <!-- Header -->
  <DCHeader></DCHeader>
  <!-- // Header -->

  <!-- Main -->
  <DCMain></DCMain>
  <!-- // Main -->

  <!-- Footer -->
  <DCFooter></DCFooter>
  <!-- // Footer -->
</template>