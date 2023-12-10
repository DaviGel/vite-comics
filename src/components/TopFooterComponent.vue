<script>
export default {
  name: 'MenuComponent',
  data() {
    return {
      comics: [
        'Characters',
        'Comics',
        'Movies',
        'TV',
        'Games',
        'Collectibles',
        'Videos',
        'Fans',
        'News',
      ],
      shop: ['Shop DC', 'Shop DC Collectibles'],
      dc: [
        'Terms',
        'Privacy policy',
        'Ad Choises',
        'Advertising',
        'Jobs',
        'Subscriptions',
        'Talent Workshops',
        'CPS Certificates',
        'Ratings',
        'Shop help',
        'Contact US',
      ],
      sites: ['DC', 'MAD Magainze', 'DC Kids', 'DC Universe', 'DC Power Visa'],
    };
  },
};
</script>

<template>
  <div class="top-footer">
    <div class="container">
      <ul>
        <li class="t-upper"><h2>DC Comics</h2></li>
        <li v-for="link in comics">
          <a href="#">{{ link }}</a>
        </li>
        <li class="t-upper"><h2>Shop</h2></li>
        <li v-for="link in shop">
          <a href="#">{{ link }}</a>
        </li>
      </ul>
      <ul>
        <li class="t-upper"><h2>DC</h2></li>
        <li v-for="link in dc">
          <a href="#">{{ link }}</a>
        </li>
      </ul>
      <ul>
        <li class="t-upper"><h2>Sites</h2></li>
        <li v-for="link in sites">
          <a href="#">{{ link }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
.top-footer {
  background-image: url('../../img/footer-bg.jpg');
  .container {
    background-image: url('../../img/dc-logo-bg.png');
    background-position: right;
    background-repeat: no-repeat;
    padding: 45px 0 60px 0;
    display: flex;
    gap: 30px;
    ul {
      li {
        list-style: none;
        color: #959595;
        h2 {
          color: #fff;
          margin: 26px 0 22px 0;
        }
        a {
          text-decoration: none;
          color: inherit;
        }
      }
    }
  }
}
</style>
