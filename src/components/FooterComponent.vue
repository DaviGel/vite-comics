<script>
import TopFooterComponent from './TopFooterComponent.vue';
import BottomFooterComponent from './BottomFooterComponent.vue';

export default {
  name: 'FooterComponent',

  components: {
    TopFooterComponent,
    BottomFooterComponent,
  },
};
</script>

<template>
  <footer>
    <TopFooterComponent />
    <BottomFooterComponent />
  </footer>
</template>

<style scoped></style>
