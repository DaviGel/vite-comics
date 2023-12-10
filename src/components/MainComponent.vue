<script>
import AzureBannerComponent from './AzureBannerComponent.vue';

export default {
  name: 'MainComponent',
  components: {
    AzureBannerComponent,
  },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="content">-> Content goes here &lt;-</div>
    </div>
    <div class="azure-banner">
      <AzureBannerComponent />
    </div>
  </main>
</template>

<style scoped lang="scss">
main {
  .azure-banner {
    background-color: #0282f9;
    height: 155px;
    display: flex;
    align-items: center;
  }
  .content {
    color: #fff;
    font-size: 24px;
    line-height: 130px;
  }
  background-color: #1c1c1c;
}
</style>
