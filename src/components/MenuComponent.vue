<script>
export default {
  name: 'MenuComponent',
  data() {
    return {
      list: [
        'Characters',
        'Comics',
        'Movies',
        'TV',
        'Games',
        'Collectibles',
        'Videos',
        'Fans',
        'News',
        'Shop',
      ],
    };
  },
};
</script>

<template>
  <ul>
    <li v-for="link in list">{{ link }}</li>
  </ul>
</template>

<style scoped></style>
