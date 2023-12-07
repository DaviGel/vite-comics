<script>
import LogoComponentVue from './LogoComponent.vue';
import MenuComponent from './MenuComponent.vue';

export default {
  name: 'HeaderComponent',
  components: {
    LogoComponentVue,
    MenuComponent,
  },
};
</script>

<template>
  <header>
    <LogoComponentVue />
    <MenuComponent />
  </header>
</template>

<style scoped></style>
