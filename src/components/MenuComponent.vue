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
    <li v-for="link in list" class="t-upper">
      <a href="#">{{ link }}</a>
    </li>
  </ul>
</template>

<style scoped lang="scss">
ul {
  display: flex;

  li {
    list-style: none;
    margin-left: 35px;
    border-bottom: 5px solid transparent;
    &:hover {
      border-bottom: 5px solid #0282f9;
    }
  }
  a {
    all: unset;
    cursor: pointer;
    &:hover {
      color: #0282f9;
    }
  }
}
</style>
