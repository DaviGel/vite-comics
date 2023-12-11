<script>
export default {
  name: 'CardComponent',
  props: {
    cards: Array,
    thumbs: String,
    series: String,
  },
};
</script>

<template>
  <ul>
    <li v-for="card in cards">
      <img :src="card.thumbs" :alt="card.series" />
      <div class="caption">{{ card.series }}</div>
    </li>
  </ul>
</template>

<style scoped lang="scss"></style>
