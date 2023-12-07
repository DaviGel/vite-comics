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
  <h2>DC Comics</h2>
  <ul>
    <li v-for="link in comics">{{ link }}</li>
  </ul>
  <h2>Shop</h2>
  <ul>
    <li v-for="link in shop">{{ link }}</li>
  </ul>
  <h2>DC</h2>
  <ul>
    <li v-for="link in dc">{{ link }}</li>
  </ul>
  <h2>Sites</h2>
  <ul>
    <li v-for="link in sites">{{ link }}</li>
  </ul>
</template>

<style scoped></style>
