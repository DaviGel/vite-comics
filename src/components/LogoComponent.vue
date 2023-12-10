<script>
export default {
  name: 'LogoComponent',
  data() {
    return {
      path: '../../img/dc-logo.png',
      title: 'dc-logo',
    };
  },
};
</script>

<template>
  <img :src="path" :alt="title" />
</template>

<style scoped lang="scss">
img {
  border-bottom: 5px solid transparent;
}
</style>
