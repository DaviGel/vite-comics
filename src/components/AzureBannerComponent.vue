<script>
export default {
  name: 'AzureBannerComponent',
  data() {
    return {
      elements: [
        {
          path: '../../img/buy-comics-digital-comics.png',
          caption: 'digital comics',
          alt: 'digital comics',
        },
        {
          path: '../../img/buy-comics-merchandise.png',
          caption: 'dc merchandise',
          alt: 'comics merchandise',
        },
        {
          path: '../../img/buy-comics-shop-locator.png',
          caption: 'subscription',
          alt: 'shop locator',
        },
        {
          path: '../../img/buy-comics-subscriptions.png',
          caption: 'comic shop locator',
          alt: 'subscriptions',
        },
        {
          path: '../../img/buy-dc-power-visa.svg',
          caption: 'dc power visa',
          alt: 'power visa',
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <ul class="t-upper">
      <li v-for="obj in elements">
        <img :src="obj.path" :alt="obj.alt" />
        <div>{{ obj.caption }}</div>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.container {
  padding: 0 43px;
  ul {
    display: flex;
    gap: 77px;
    li {
      list-style: none;
      display: flex;
      align-items: center;
      color: #fff;
      font-size: 13px;
      img {
        width: 44px;
        height: 55px;
        object-fit: contain;
        margin-right: 15px;
      }
    }
  }
}
</style>
