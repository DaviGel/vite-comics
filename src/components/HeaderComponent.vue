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
    <div class="container">
      <LogoComponentVue />
      <MenuComponent />
    </div>
  </header>
</template>

<style scoped lang="scss">
header {
  height: 117px;
  line-height: 117px;
  margin: 5px;
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
