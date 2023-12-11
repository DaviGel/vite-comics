<script>
export default {
  name: 'CardComponent',
  props: {
    cards: Array,
    thumb: String,
    series: String,
  },
};
</script>

<template>
  <div class="btn current t-upper">
    <button>Current series</button>
  </div>
  <ul>
    <li v-for="card in cards">
      <img :src="card.thumb" :alt="card.series" />
      <div class="caption">{{ card.series }}</div>
    </li>
  </ul>
  <div class="btn t-upper">
    <button>Load More</button>
  </div>
</template>

<style scoped lang="scss">
img {
  width: 200px;
  height: 200px;
  object-fit: cover;
}
ul {
  display: flex;
  flex-wrap: wrap;
  gap: 29px;
  padding: 3.125rem 0 3.125rem 0;
  li {
    list-style: none;
    width: calc(100% / 6 - 29px);
    div {
      color: #f8f4f8;
    }
  }
}
.btn {
  text-align: center;
  margin-bottom: 20px;
  button {
    all: unset;
    cursor: pointer;
    background-color: #0282f9;
    color: white;
    padding: 10px 60px;
  }
  &.current {
    font-size: 26px;
    text-align: left;
    position: relative;
    top: -28px;
    left: -14px;
  }
}
</style>
