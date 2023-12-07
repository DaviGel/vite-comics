<script>
export default {
  name: 'BottomFooterComponent',
  data() {
    return {
      iconPath: [
        '../../img/footer-facebook.png',
        '../../img/footer-periscope.png',
        '../../img/footer-pinterest.png',
        '../../img/footer-twitter.png',
        '../../img/footer-youtube.png',
      ],
    };
  },
};
</script>

<template>
  <div class="left-content"><button>Sign-up now</button></div>
  <div class="righ-content">
    <span>Follow us</span>
    <ul>
      <li v-for="(path, index) in iconPath">
        <img :src="path" :alt="index" />
      </li>
    </ul>
  </div>
</template>

<style scoped></style>
